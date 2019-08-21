#!/bin/bash

aws iam create-role --role-name kubernetes-master-role --assume-role-policy-document file:kubernetes-master-role.json
aws iam put-role-policy --role-name kubernetes-master-role --policy-name vmimport --policy-document file://kubernetes-master-policy.json


aws iam create-role --role-name kubernetes-minion-role --assume-role-policy-document file://kubernetes-minion-role.json
aws iam put-role-policy --role-name kubernetes-minion-role --policy-name vmimport --policy-document file://kubernetes-minion-policy.json

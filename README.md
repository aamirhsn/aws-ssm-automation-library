# AWS SSM Automation Library
This repository contains a collection of AWS SSM automation documents to help automate common operational, compliance and migration related tasks in AWS environment.

### Runbook information:
| Document Name                          | Description |
|----------------------------------------|--------------------------------------------------------------------|
| **ec2-remove-public-ip.yaml** | Removes public IPs from all EC2 instances |
| **ec2-join-domain.json** | Join EC2 instances to an Active Directory |
| **aws-tag-resources.yaml** | Tags AWS resources based on defined parameters |
| **ssm-patch-tuesday-mw-schedule.yaml** | Updates SSM Maitenance Window schedule to align with Patch Tuesday |
| **ssm-import-export-parameters.yaml** | Imports/Exports SSM Parameters | 
| **mgn-pre-post-migration-analysis.yaml** | Performs Pre and Post Migration validation checks and compares them (Windows OS only) |

### Usage:
1. Clone or download the desired yaml/json file and create the SSM document using AWS CLI or Console.
   ```
   aws ssm create-document --name "DocumentName" --document-type "Automation" --content file://DocumentName.yaml
   ```

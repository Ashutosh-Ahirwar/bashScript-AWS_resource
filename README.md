# AWS Resource Listing Script

## Description

This script lists various AWS resources in a specified AWS region. 

**Author:** Ashutosh  
**Version:** v0.0.1

## Supported Services

- EC2
- S3
- RDS
- DynamoDB
- EBS
- Lambda
- ELB
- CloudFront
- CloudWatch
- SNS
- SQS
- Route53
- VPC
- CloudFormation
- IAM

## Usage

```bash
./script.sh <region> <service_name>
```
## Example

```bash
./script.sh ap-south-1 EC2
```
## Requirements

- AWS CLI installed and configured

## Script Details

- **Check for Valid Arguments:** Ensures that the correct number of arguments is provided.
- **AWS CLI Installation Check:** Verifies that the AWS CLI is installed.
- **AWS CLI Configuration Check:** Verifies that the AWS CLI is configured.
- **List Resources:** Based on the service name, lists the corresponding AWS resources.

## Supported Services and Commands

- **EC2:** `aws ec2 describe-instances`
- **S3:** `aws s3api list-buckets`
- **RDS:** `aws rds describe-db-instances`
- **CloudFront:** `aws cloudfront list-distributions`
- **VPC:** `aws ec2 describe-vpcs`
- **IAM:** `aws iam list-users`
- **Route53:** `aws route53 list-hosted-zones`
- **CloudWatch:** `aws cloudwatch describe-alarms`
- **CloudFormation:** `aws cloudformation describe-stacks`
- **Lambda:** `aws lambda list-functions`
- **SNS:** `aws sns list-topics`
- **SQS:** `aws sqs list-queues`
- **DynamoDB:** `aws dynamodb list-tables`
- **EBS:** `aws ec2 describe-volumes`

## Error Handling

- **Invalid Arguments:** Displays usage information.
- **AWS CLI Not Installed:** Prompts to install the AWS CLI.
- **AWS CLI Not Configured:** Prompts to configure the AWS CLI.
- **Invalid Service:** Displays an error for an unsupported service.

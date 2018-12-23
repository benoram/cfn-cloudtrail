# CloudFormation Template for CloudTrail

## Purpose

This template (cfn-cloudtrail.yaml) is designed to be used in a single AWS account. The script creates an S3 bucket, and CloudTrail enabled for all regions. Optionally you can enable SNS to publish notifications when new log files arrive, and you can enable CloudWatch logs to push logs into CloudWatch.

Finally, the template sets a bucket policy that prevents all users except root from deleting log files from S3.

The script takes care of everything needed for log expiration, and ultimate deletion.

## Dependencies

Amazon Services
- CloudTrail
- S3
- IAM
- SNS (optional)
- CloudWatch Logs (optional)
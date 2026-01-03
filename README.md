# Automated AWS S3 Bucket Cost Optimization Framework with EventBridge Scheduler, Lambda, SNS, and IAM



## For more projects, check out  
[https://harishnshetty.github.io/projects.html](https://harishnshetty.github.io/projects.html)

[![Video Tutorial](https://github.com/harishnshetty/image-data-project/blob/ccd5b46f956ad4cea6b16d3e03c9b2a236ecb107/stale-s3.jpg)](https://youtu.be/BgyYqUXuHuk?si=Gi6vkxhnVJQBILkG)


## Production-Grade S3 Bucket Auto Delete System for Cost Optimization Using AWS Serverless Services


### lambda time out
5 min  
Runtime python3.14

### IAM ROLE inline policy

- "s3:ListAllMyBuckets",
- "s3:ListBucketVersions",
- "s3:ListBucket",
- "s3:DeleteBucket"
- "sns:Publish"

## IAM ROLE inline policy
- CloudWatchFullAccess
- CloudWatchFullAccessV2



### start scheduler
`00 8 ? JAN-DEC FRI *`

### Delete the resources

1. delete the lambda function
2. delete the iam role
3. delete the event bridge scheduler
4. delete the sns topic
5. delete the s3 buckets
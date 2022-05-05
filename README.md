# WEBSPARK
### Test task:
1. Create an AWS CloudFormation configuration file that uses arguments
```

Parameters:
  DomainName:
    Type: String
    Description: The DNS name of an existing Amazon Route 53 hosted zone
  BucketName:
    Type: String
    Description: Amazon S3 files bucket name
  HostedZoneId:
    Type: String
    Description: Amazon Route53 Hosted Zone Id
  CertificateArn:
    Type: String
    Description: Certificate Link
```
2. After applying the configuration, the following resources must be created and configured:
* S3 bucket
* S3 policy
* CloudFront distribution for S3 files bucket
* Route53 A-record to the CloudFront files distribution

The output should show:
* created by ID CloudFront

### To execute, go to the directory with the file and run the command:
```

aws cloudformation deploy --stack-name webspark-tw --template-file thrid.yaml
```

 
 



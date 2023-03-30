# MOS Validation Server (v2) Infrastructure

This repository contains the CloudFormation stack for the non-serverless validation server prototype (v2) infrastructure (i.e. KMS key, RDS, web server, IAM user for the API). 

To deploy (requires [AWS CLI](https://aws.amazon.com/cli/) to be installed and configured):

```bash
./deploy.sh
```

This requires an `.env` file with the following variables set:

```
BACKEND_MASTER_USER_PASSWORD
DBPrivateSubnet
DBSecurityGroup
S3BucketName
VpcId
Region
EC2PublicSubnet
EC2SecurityGroup
Tag-Name
Tag-Project-Name
Tag-Project-Code
Tag-Tech-Team
Tag-Center
Tag-Requested-By
Tag-Created-By
Tag-Platform
```

## Infrastructure for Middleware/Front-end
<img width="1335" alt="Screen Shot 2022-11-29 at 1 14 50 PM" src="https://user-images.githubusercontent.com/9484180/204624822-1d17ffa0-a859-42f2-9244-e207d2064dad.png">
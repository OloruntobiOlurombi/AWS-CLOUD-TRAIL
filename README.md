# TOPIC: AWS-CLOUD-TRAIL

### Overview
> AWS CloudTrail is an AWS service that helps you enable governance, compliance, and operational and risk auditing of your AWS account. Actions taken by a user, role, or an AWS service are recorded as events in CloudTrail. Events include actions taken in the AWS Management Console, AWS Command Line Interface, and AWS SDKs and APIs.

> CloudTrail is enabled on your AWS account when you create it. When activity occurs in your AWS account, that activity is recorded in a CloudTrail event. You can easily view recent events in the CloudTrail console by going to Event history.

### Prerequisites: 
> AWS Account

### Steps to create a CloudTrail

### Step 1: Access CloudTrail Dashboard
> Navigate to [the CloudTrail dashboard](https://us-east-1.console.aws.amazon.com/cloudtrail/home?region=us-east-1#), and launch the wizard to create a trail.

![image](https://user-images.githubusercontent.com/40290711/170471305-acd49cda-444d-41ef-9811-b80c8e8b38f1.png)

### Step 2: Create a Trail

> AWS provides a quick trail create process, where you just have to specify the display name for your trail, and an S3 bucket to store logs.

> 1. Quick process
> The Quick trail create wizard will automatically create an S3 bucket and folder on your behalf to store the logs. The folder in the newly created S3 bucket is aws-cloud trail-logs-014421265158-1acfb819, and the folder is AWSLogs/014421265158/CloudTrail/. It will create further sub-folders based on your region name, year, month, and date. An example (auto-generated) file created at the above mention path in the S3 bucket is:

014421265158_CloudTrail_us-east-1_20201126T1225Z_AumNC3WbMzJTBiSR.json.gz

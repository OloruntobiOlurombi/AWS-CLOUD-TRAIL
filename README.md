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
> The Quick trail create wizard will automatically create an S3 bucket and folder on your behalf to store the logs. The folder in the newly created S3 bucket is aws-cloud trail-logs-014421265158-1acfb819, and the folder is AWSLogs/014421265158/CloudTrail/. It will create further sub-folders based on your region name, year, month, and date. An example (auto-generated) file created at the above mention path in the S3 bucket is: 014421265158_CloudTrail_us-east-1_20201126T1225Z_AumNC3WbMzJTBiSR.json.gz.

![image](https://user-images.githubusercontent.com/40290711/170473227-ea20be83-7bae-4112-b217-ad2eba8ac27b.png)

![image](https://user-images.githubusercontent.com/40290711/170473717-b0350c03-05d1-48cb-9ffb-fc5a633a5fd8.png)

> 3. Regular process
> If you wish to use an existing S3 bucket, you will have to navigate to the detailed Create trail process. You can launch one from the CloudTrail dashboard. The regular Create trail is a three-step process:

> Step 1 - General details - Provide the trail name, choose the new/existing S3 bucket, and enable/disable the encryption.

> If the encryption is enabled, CloudTrail will encrypt log files by using the AWS Key Management Service (SSE-KMS). In addition, you can choose to be notified each time a log is delivered to your bucket. There is another feature, log digest, to verify that your log files did not change after CloudTrail delivered them.

![image](https://user-images.githubusercontent.com/40290711/170474555-bf8cf23d-67e8-47eb-afbe-fede6cc700e9.png)


> Step 2 - Events and Management details - Choose the types of events you want to log. There are three categories of events - Management events, Data events (operations performed within a resource), and Insights events (unusual activity, errors, or user behavior).

![image](https://user-images.githubusercontent.com/40290711/170475085-71d41ce5-e8fa-4cad-8dfa-1958f68f9617.png)

> Step 3 - Review and Create 

![image](https://user-images.githubusercontent.com/40290711/170475500-59e0812d-5ca4-4270-8f41-5ade19035d2d.png)

![image](https://user-images.githubusercontent.com/40290711/170475904-1c61837a-872e-465f-9389-86d3e0f54e27.png)


### Step 3: Dashboard

> The CloudTrail dashboard displays an overview of all your trails, insights, and event history.

> Consider a Trail as a log of all the events/actions that occurred in your AWS account. Of course, events have to be processed to convert them into a particular log-format.

![image](https://user-images.githubusercontent.com/40290711/170476994-3dc8435d-5d7c-4fa2-8744-a16098919f5d.png)

- In the snapshot above, notice the separate table for Trails, Insights, and Event history. The Event history section shows all the recent events. It shows every action that occurred in your AWS account. Click on View full Event history to see additional details and more events that have occurred.

- Remember, that the first trail does not attract billing charges. However, you incur charges for the S3 bucket that will store your logs. You can create additional trails on a charge-basis.

![image](https://user-images.githubusercontent.com/40290711/170477277-1b6e4f3c-8a83-43db-9a7c-824ecc35ab90.png)

# The End 


# Auto-Tagging-In-AWS
Code to Implement Dynamic Auto-Tagging in AWS
This AWS Lambda Code Uses: AWS CloudWatch Event Rule, AWS CloudTrail and AWS S3.
////////////////////////////////////////////////////////////
The Lambda Code Applies Tags Automatically to the Resources as per the Data (Tags) mentioned Against each username in a CSV File that is kept stored in an S3 Bucket. So if "Rahul" Creates an Instance in EC2, the lambda function wll get triggered        automatically, the lambda code will get the username of Rahul from AWS CloudTrail Environment and it will get the content of CSV File from S3 Bucket then it will match Rahul's Username in the CSV and get the corresponding Tag Value Mentioned in the CSV File. And then it will apply the tag to the resource (EC2 Instance here) created by Rahul.
////////////////////////////////////////////////////////////

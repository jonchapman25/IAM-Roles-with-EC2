Lab 2: IAM Roles with EC2 — Secure S3 Access

Objective
Demonstrate how to securely allow an EC2 instance to access Amazon S3 without using access keys by using IAM roles.
 Steps Completed
![description](https://i.imgur.com/9a89m70.png)
1. Created an IAM role specifically for EC2 instances.  
2. Attached the AmazonS3ReadOnlyAccess policy to enforce read-only access to S3 buckets.  
3. Launched an EC2 instance with the IAM role attached.  
4. Connected to the EC2 instance via Session Manager/SSH.  
5. Verified access by running:
   ```bash
   aws s3 ls

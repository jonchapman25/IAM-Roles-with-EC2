Lab 2: IAM Roles with EC2 — Secure S3 Access

Objective:

Demonstrate how to securely allow an EC2 instance to access Amazon S3 without using access keys by using IAM roles.
 
Steps Completed:

1. Created an IAM role specifically for EC2 instances.
![Description](https://i.imgur.com/9a89m70.png)

2. Attached the AmazonS3ReadOnlyAccess policy to enforce read-only access to S3 buckets.  
![Description](https://i.imgur.com/9wYMzo6_d.webp?maxwidth=1520&fidelity=grand)

3. Launched an EC2 instance with the IAM role attached.  
![Description](https://i.imgur.com/Yuq1K9f_d.webp?maxwidth=1520&fidelity=grand)

4. Connected to the EC2 instance via Session Manager/SSH.  
![Description](https://i.imgur.com/P3BAOHI_d.webp?maxwidth=760&fidelity=grand)

5. Verified access by running:
   ```bash
   aws s3 ls
![Description](https://i.imgur.com/A7cSUt0_d.webp?maxwidth=760&fidelity=grand)
# AWS IAM Session Questions and Answers

### 1. Which is AWS's responsibility under the AWS shared responsibility model?
- **Answer**: Maintaining physical hardware

### 2. Which is a best practice in IAM concerning the root user?
- **Answer**: Do not use root account credentials for day-to-day interactions with AWS.

### 3. An IAM policy that allows access to an Amazon S3 bucket is attached to an IAM user. The Amazon S3 bucket has a bucket policy that denies the IAM user access to the bucket.  
Which statement is true about the conflicting IAM and resource policies?
- **Answer**: A policy with a deny statement overrides an allow statement. The IAM user cannot access the bucket.

### 4. Which service would you use to authenticate and authorize users on your web application?
- **Answer**: Amazon Cognito

### 5. Which section on the IAM policy statement determines whether the user's access is being denied or allowed?
- **Answer**: Effect

### 6. Which two services are designed specifically for data protection? (Choose TWO.)
- **Answer**: Secrets Manager, AWS KMS

### 7. Which statement is true in regards to what is required for a user to assume a role?
- **Answer**: The user needs to be defined as the principal that you trust to assume the role in the trust policy.

### 8. You want an added layer of security to authenticate a user when the user logs in. What should you do?
- **Answer**: Enable multi-factor authentication (MFA) on the IAM user's account

### 9. Which service helps protect your application on AWS from DDOS attacks?
- **Answer**: Shield

### 10. What can you do in IAM to help you evaluate whether the principle of least privileged is being enforced? (Choose TWO.)
- **Answer**: 
  - Provide the IAM user with a limited set of permissions and increase as needed.
  - Use the IAM Access Analyzer to help fine-grain the IAM users' permissions.

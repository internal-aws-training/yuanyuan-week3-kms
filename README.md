# Homework - week3 

### 1. What is KMS , and KMS can handle which problems?
KMS is AWS Key Management Service, can be used to create and control *customer master keys* (CMKs), and  CMK is the encryption keys used to encrypt your data.

### 2. The approaches to use KMS.

- Perform these AWS Key Management Service (AWS KMS) tasks in[AWS Management Console](https://console.aws.amazon.com/iam/).
-  Access all AWS KMS features by using the [AWS KMS API operations](https://docs.aws.amazon.com/kms/latest/APIReference/).
- To run the AWS KMS API operations, use [AWS SDK](https://aws.amazon.com/tools/#sdk)
- Use [AWS Command Line Interface](https://aws.amazon.com/tools/#cli) (AWS CLI) or [AWS Tools for PowerShell](https://docs.aws.amazon.com/powershell/latest/userguide/).
- Shush tool.

### 3. You can do which action by using KMS (you should know at least  5 or more?
- Create CMK
- Enable CMK
- Disable CMK
- Encrypt data with CMK
- Decrypt date 

### 4. Practice
#### Use AWS-Cli to encrypt/decrypt
```
./auto/aws-cli/create-cmk
./auto/aws-cli/encrypt
./auto/aws-cli/decrypt
```

#### Use Shush to encrypt/decrypt 
```
./auto/shush/encrypt
./auto/shush/decrypt
```

### 5. You are the designer to use KMS in your current project, please do the scenario description or showcase (how, why etc.)

When a backend service need to connect to Database and need to save the password in code, then we can use KMS the encrypt the password as a encrypted-password.
And before the service connect to db, decrypt the encrypted-password first. 

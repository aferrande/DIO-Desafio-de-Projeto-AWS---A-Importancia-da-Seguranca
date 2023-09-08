# REPORT ON THE IMPLEMENTATION OF SAFETY MEASURES

Date: 09/04/2023
Company: Abstergo Industries
Responsible: Arthur de Assis Ferrande

## Introduction
This report presents the tool implementation process at Abstergo Industries, carried out by Arthur de Assis Ferrande. The objective of the project was to list security measures in conjunction with AWS services, in order to increase security in the company.

## Project description
The tool implementation project was divided into 3 security measures. The implementation steps are described below:

Measure 1:
- Use IAM to create users, user groups, roles, policies, among others. No longer needing to use the root account to carry out tasks, this makes it easier to manage and control access, and increases security in general. With the concept of granularity and least-privilege, we prevent a user or application from having access to any resource that is not necessary to carry out their activities, protecting us from possible malicious actions, or even human error. We can, for example, remove permission from a role or user to delete/stop an instance, thus ensuring greater control over functions and actions within applications.
It is also important to define the need to create a strong password for users, which together with MFA (Multi-Factor Authentication) adds another layer of security in case a user loses their password or has their credentials exposed or stolen. Another interesting practice is to put an expiration time for credentials and passwords.

Measure 2:
- Use encryption and AWS Key Management Service to create encrypted keys to access data at rest or in transit contained in our databases or storage. Avoiding the risk of this data being accessed by unauthorized persons.

Measure 3:
- We can use resources such as AWS WAF, AWS GuardDuty, among others, to increase the network security of our applications. Protecting against attacks and exploits, from SQL injection to a brute force attack for information theft.

Measure 4:
- Use Amazon Inspector to check possible vulnerabilities and necessary updates in our resources, such as an operating system on an EC2 instance.

Measure 5:
- Use CloudWatch and CloudTrail to generate logs and alarms, thus being able to visualize and record actions committed in our applications. These logs are sent to an S3 bucket, which also needs to be secure. That is, restricted and non-public access, and we can add the need for MFA to delete such a bucket.

## Conclusion
The implementation of tools in the company Abstergo Industries is expected to increase the security of resources and applications against external attacks and unauthorized access, such as that of users themselves by protecting their access credentials. It is recommended to continue using the implemented tools and search for new technologies that can further improve the company's processes.

## Attachments

https://aws.amazon.com/en/products/security/
https://docs.aws.amazon.com/iam/
https://docs.aws.amazon.com/kms/
https://docs.aws.amazon.com/guardduty/
https://docs.aws.amazon.com/waf/
https://aws.amazon.com/pt/inspector/
https://aws.amazon.com/pt/cloudwatch/
https://aws.amazon.com/en/cloudtrail/
https://aws.amazon.com/pt/s3/

Signature of the Person Responsible for the Project:

Arthur de Assis Ferrande

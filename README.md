# IAM Roles and Access Management – AWS

## 1. Project Overview

This project demonstrates secure access management using AWS Identity and Access Management (IAM). It focuses on managing users, groups, roles, and permissions to ensure secure access to AWS resources.

The project follows the Principle of Least Privilege to provide users and services with only the permissions they need.

## 2. Project Objectives

- Understand AWS IAM and its importance.
- Create and manage IAM users.
- Organize users into IAM groups.
- Attach permission policies.
- Create IAM roles for AWS services.
- Implement role-based access control.
- Understand secure access management.

## 3. AWS Services Used

- AWS Identity and Access Management (IAM)
- Amazon Simple Storage Service (S3)
- Amazon Elastic Compute Cloud (EC2)

## 4. Project Implementation

### Task 1: Create IAM User
- Created an IAM user named `server`.
- Configured the user account.

### Task 2: Create IAM Group
- Created an IAM group named `Server-Group`.
- Added the IAM user `server` to the group.

### Task 3: Attach IAM Policy
- Attached `AmazonS3ReadOnlyAccess` to the group.
- Provided read-only access to Amazon S3 resources.

### Task 4: Create IAM Role
- Created an IAM role named `EC2-S3-Access-Role`.
- Selected EC2 as the trusted AWS service.
- Attached the `AmazonS3ReadOnlyAccess` policy.

### Task 5: Verify Permissions
- Verified IAM user group membership.
- Checked the attached permissions.
- Verified the IAM role configuration and trust relationship.

## 5. Project Architecture

IAM User (server)  
↓  
IAM Group (Server-Group)  
↓  
IAM Policy (AmazonS3ReadOnlyAccess)

EC2 Instance  
↓  
IAM Role (EC2-S3-Access-Role)  
↓  
IAM Policy (AmazonS3ReadOnlyAccess)  
↓  
Amazon S3

## 6. Security Best Practices

- Followed the Principle of Least Privilege.
- Used IAM groups to manage permissions.
- Used IAM roles for AWS service access.
- Avoided storing access keys on EC2 instances.
- Applied read-only permissions where appropriate.

## 7. Key Learnings

- Understanding AWS IAM users, groups, roles, and policies.
- Managing access permissions securely.
- Understanding role-based access control.
- Learning how EC2 can access AWS services through IAM roles.

## 8. Conclusion

Successfully configured an AWS IAM access management setup using users, groups, roles, and policies. This project provided practical knowledge of AWS identity management and cloud security fundamentals.

## 9. Screenshots

Add your project screenshots here:

1. IAM Dashboard
2. IAM User – server
3. IAM Group – Server-Group
4. IAM Policy Permissions
5. EC2-S3-Access-Role
6. Role Trust Relationship

**Project Domain:** AWS Cloud Computing  
**Project Type:** Hands-on AWS Project  
**Tools:** AWS Management Console, IAM, S3, EC2

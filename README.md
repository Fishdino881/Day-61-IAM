# Day-61-IAM

###  Overview

**AWS IAM (Identity and Access Management)** is a service that helps you **securely control access to AWS resources**.

It allows you to create users, groups, and roles and assign permissions to determine **who can access what resources** in AWS.

---

##  Key Components of IAM

###  Users

An **IAM user** represents a person or application that interacts with AWS.

Example:

* Developer
* Data engineer
* Application service

Each user has unique login credentials.

---

###  Groups

Groups are collections of IAM users.

Instead of assigning permissions to each user individually, permissions can be applied to **groups**.

Example groups:

* Admin
* Developers
* Data Analysts

---

###  Roles

An **IAM role** allows temporary access to AWS resources.

Roles are commonly used by:

* Applications
* AWS services
* Cross-account access

---

###  Policies

Policies define **permissions** in JSON format.

Example policy structure:

```json
{
 "Effect": "Allow",
 "Action": "s3:ListBucket",
 "Resource": "*"
}
```

Policies specify:

* Allowed or denied actions
* AWS resources
* Conditions

---

##  Real-World Use Cases

* Restricting access to sensitive data
* Managing developer permissions
* Securing production environments
* Controlling access to S3, EC2, and other services


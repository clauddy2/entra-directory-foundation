
Microsoft Entra ID – Directory Foundation Lab
Project Overview

In this lab, I built a Microsoft Entra ID environment for Northwind Services, a fictional small company. My goal was to practice creating and managing users, organizing users into security groups, and applying basic IAM and access management concepts.

What I Did
1. Designed the User Structure

Before creating the accounts, I created a user list showing each employee's:

Name and UPN
Job Title
Department
Manager
Usage Location
Group Membership

I used a consistent naming convention for my security groups, such as SEC-Department-Sales and SEC-Role-Helpdesk.

2. Created Users

I created the first 5 users manually in Microsoft Entra ID to understand the user creation process and the different user properties.

I then used Microsoft's Bulk Create CSV template to create the remaining users. I also added a newly hired Sales employee, bringing the environment to 16 users.

3. Created Security Groups

I created department-based security groups to organize users and make access easier to manage:

SEC-Department-IT
SEC-Department-Finance
SEC-Department-Sales
SEC-Department-HR
SEC-Department-Contractors

I used Security as the group type and Assigned membership.

4. Created a Role-Based Group

I created SEC-Role-Helpdesk to practice managing access based on job responsibilities instead of department.

This helped me understand how a user can belong to a department group while also belonging to another group based on the work they perform.

5. Managed Contractor Access

I separated contractors from regular employees using SEC-Department-Contractors. This allows contractor access to be managed and reviewed separately, especially when a contract ends.

6. Verified My Work

After completing the configuration, I reviewed the Microsoft Entra audit logs to verify user creation, group creation, and membership changes.

I also captured screenshots of my users, groups, group memberships, user properties, and audit logs as evidence of the work completed.

What I Learned

This lab gave me hands-on experience with Microsoft Entra ID user provisioning, bulk user creation, security groups, RBAC concepts, identity lifecycle management, least privilege, and audit logging.

Most importantly, I learned why managing access through groups instead of individual users makes IAM easier to manage, audit, and scale.


## Microsoft Entra ID Lab Screenshots

The screenshots below demonstrate the Microsoft Entra ID tasks completed during this lab.

### Users List
![Users List](screenshots/https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/users%20list-screenshot.PNG)

### User Details
![User Details](screenshots/https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/user's%20detail-screenshot.PNG)

### Groups List
![Groups List](screenshots/https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/groups%20list-screenshot.PNG)

### Group Members
![Group Members](screenshots/https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/group's%20members-screenshot.PNG)

### Audit Logs

#### Audit Log - Screenshot 1
![Audit Logs Screenshot 1](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/audit%20logs-screenshot1.PNG)

#### Audit Log - Screenshot 2
![Audit Logs Screenshot 2](screenshots/https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/audit%20logs-screenshot2.PNG)

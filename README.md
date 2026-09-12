
**Microsoft Entra ID – Directory Foundation Project Overview**

**Northwind – Microsoft Entra ID IAM Project Overview**

In this project, I built and configured a Microsoft Entra ID environment for Northwind Services, a fictional 15-person company. The objective was to gain hands-on experience with identity and access management (IAM), including user provisioning, security groups, role-based access, contractor management, identity lifecycle concepts, and audit logging.

During the project, I also onboarded a newly hired Sales employee, increasing the environment from 15 to 16 users.

**Designed the User Structure**

Before creating accounts in Microsoft Entra ID, I designed a user structure for Northwind Services. I documented each user's name, User Principal Name (UPN), job title, department, manager, usage location, and required group membership.

I also established a consistent security-group naming convention:

SEC-<Type>-<Name>

Examples:

SEC-Department-Sales
SEC-Department-IT
SEC-Role-Helpdesk

This provided a structured approach for managing identities and access as the organization grows.

**Created and Provisioned Users**

I manually created five users in Microsoft Entra ID. This allowed me to become familiar with the user creation process and properties such as UPN, job title, department, manager, and usage location.

After validating the process, I used Microsoft's Bulk Create CSV template to provision the remaining users more efficiently.

I later added a newly hired employee to the Sales department, increasing the environment to 16 users.

**Created Department-Based Security Groups**

I created security groups to organize users according to their departments:

SEC-Department-IT
SEC-Department-Finance
SEC-Department-Sales
SEC-Department-HR
SEC-Department-Contractors

I configured them as Security groups with Assigned membership and added the appropriate users to each group.

Using department groups demonstrated how access can be managed centrally rather than assigning permissions separately to every employee.

**Created a Role-Based Helpdesk Group**

I created the SEC-Role-Helpdesk security group to practice managing access according to job responsibilities rather than department.

This demonstrated how a user can belong to a department group while also being assigned to a separate role-based group based on the work they perform.

For example:

User → Department Group → Role-Based Group → Access

This introduced me to practical concepts associated with Role-Based Access Control (RBAC) and least-privilege access.

**Separated Contractor Access**

I placed contractors into a dedicated SEC-Department-Contractors security group rather than treating them as regular employees.

Separating contractors makes their access easier to identify, review, and remove when their contracts expire. This helped me understand the importance of identity lifecycle management, especially for temporary and non-employee identities.

**Verified Group Membership and User Properties**

After creating the users and groups, I reviewed the configuration to confirm that users had the correct:

Department
Job title
Manager
Usage location
Security group membership

I also verified that department and role-based memberships aligned with the original Northwind user design.

**Reviewed Entra ID Audit Logs**

I reviewed the Microsoft Entra ID audit logs after completing the configuration.

The audit logs allowed me to verify administrative activities such as user creation, group creation, and group membership changes.

This demonstrated how audit logging provides visibility and accountability for identity-related activities within an organization.

## Microsoft Entra ID Directory Foundation - Screenshots

I captured screenshots throughout the project to provide evidence of the configuration and work completed.

### Users List
![Users List](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/users%20list-screenshot.PNG)

### User Details
![User Details](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/user's%20detail-screenshot.PNG)

### Groups List
![Groups List](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/groups%20list-screenshot.PNG)

### Group Members
![Group Members](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/group's%20members-screenshot.PNG)

### Audit Logs

#### Audit Log - Screenshot 1
![Audit Logs Screenshot 1](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/audit%20logs-screenshot1.PNG)

#### Audit Log - Screenshot 2
![Audit Logs Screenshot 2](https://github.com/clauddy2/entra-directory-foundation/blob/7a53e887f8b12acef3ea6bcad3843435363856aa/screenshots/audit%20logs-screenshot2.PNG)

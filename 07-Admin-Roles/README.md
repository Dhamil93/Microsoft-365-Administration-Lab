\# Microsoft 365 Admin Roles \& Least Privilege Lab



\## Objective



The objective of this lab was to demonstrate \*\*Role-Based Access Control (RBAC)\*\* and the \*\*principle of least privilege\*\* within Microsoft Entra ID.



The lab focused on assigning a limited administrative role to a standard user, testing the delegated permissions, and removing the administrative role after the required task was completed.



\## Environment



\* Microsoft 365 Business Premium

\* Microsoft 365 Admin Center

\* Microsoft Entra ID

\* Microsoft Entra Admin Center

\* Tenant: `PersonalLab851.onmicrosoft.com`



\## Test Account



\*\*User:\*\* John Admin

\*\*Department:\*\* IT

\*\*Job Title:\*\* IT Support Administrator



John Admin was initially configured as a standard Microsoft 365 user without administrative access.



\## Administrative Role Assigned



John Admin was temporarily assigned the:



\*\*Helpdesk Administrator\*\* role



This role provided delegated administrative capabilities appropriate for IT support activities without granting unrestricted control over the Microsoft 365 tenant.



\## Principle of Least Privilege



The \*\*Global Administrator\*\* role was deliberately avoided.



A Global Administrator has extensive control over Microsoft 365 and Microsoft Entra ID. Providing this level of access to an IT support account would grant more permissions than were necessary for the task.



Instead, the Helpdesk Administrator role was used to demonstrate the principle of least privilege:



> Users and administrators should receive only the permissions necessary to perform their required responsibilities.



\## Administrative Task Performed



After receiving the Helpdesk Administrator role, John Admin signed into the Microsoft 365 Admin Center.



A simulated help-desk scenario was performed using the \*\*Sarah HR\*\* test account.



John Admin successfully:



\* Accessed user-management functionality

\* Selected the Sarah HR account

\* Performed a password reset

\* Generated a temporary password for the user



The successful password reset demonstrated that John Admin could perform an appropriate support task using delegated administrative permissions.



No temporary password was exposed or stored in the project documentation.



\## Role Removal



After the administrative task was completed, the Helpdesk Administrator role was removed from John Admin.



This demonstrated the complete privileged-access lifecycle:



`Standard User → Administrative Role Assignment → Administrative Task → Role Removal`



Removing unnecessary administrative privileges reduces the amount of time an account maintains elevated access.



\## Tasks Completed



\* Reviewed Microsoft Entra administrative roles

\* Reviewed the capabilities of limited administrative roles

\* Assigned the Helpdesk Administrator role

\* Avoided unnecessary Global Administrator privileges

\* Tested delegated administrative access

\* Performed a user password reset

\* Verified that the delegated role allowed the required help-desk operation

\* Removed the administrative role after testing

\* Returned the test account to standard user access



\## Skills Demonstrated



\* Microsoft Entra ID administration

\* Microsoft Entra administrative roles

\* Role-Based Access Control (RBAC)

\* Principle of least privilege

\* Helpdesk Administrator role

\* Delegated administration

\* User password administration

\* Microsoft 365 user support

\* Administrative role assignment

\* Administrative role removal

\* Privileged-access lifecycle management



\## Security Considerations



Administrative privileges should only be granted when required and should provide no more access than necessary for the administrator's responsibilities.



The Global Administrator role was deliberately avoided because the test task did not require unrestricted tenant access.



The Helpdesk Administrator role provided sufficient permissions for the required support operation while reducing unnecessary administrative privileges.



After testing was completed, the elevated role was removed from the test account.



No passwords, MFA codes, authentication secrets, recovery information, or other sensitive credentials were included in the project documentation.




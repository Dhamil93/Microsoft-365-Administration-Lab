\# Exchange Online Administration Lab



\## Objective



The objective of this lab was to gain hands-on experience administering Exchange Online within Microsoft 365. The lab focused on managing user mailboxes, creating a shared mailbox, configuring mailbox delegation, adding an email alias, and testing internal email communication.



\## Environment



\* Microsoft 365 Business Premium

\* Microsoft 365 Admin Center

\* Exchange Online

\* Exchange Admin Center

\* Microsoft Outlook

\* Microsoft Entra ID

\* Tenant: `PersonalLab851.onmicrosoft.com`



\## User Mailboxes



The following Microsoft 365 user accounts were used in the Exchange Online environment:



| User            | Department      |

| --------------- | --------------- |

| John Admin      | IT              |

| Sarah HR        | Human Resources |

| Michael Finance | Finance         |

| David Sales     | Sales           |



The users were assigned Microsoft 365 Business Premium licenses, providing access to Exchange Online services.



\## Shared Mailbox



A shared mailbox was created to simulate an organization's IT help desk.



\*\*Shared Mailbox:\*\* IT Support

\*\*Primary Email:\*\* `itsupport@PersonalLab851.onmicrosoft.com`



The shared mailbox provides a centralized location where IT support requests can be received and managed without relying on an individual employee's mailbox.



\## Mailbox Delegation



Mailbox permissions were configured for \*\*John Admin\*\*, the IT Support Administrator.



The following permissions were assigned:



\* \*\*Full Access (Read and Manage)\*\* — Allows John Admin to open and manage the IT Support shared mailbox.

\* \*\*Send As\*\* — Allows John Admin to send messages that appear to originate from the IT Support shared mailbox.



This configuration demonstrates mailbox delegation and shared mailbox administration in Exchange Online.



\## Email Alias



An additional email alias was configured for the IT Support shared mailbox:



\*\*Primary address:\*\*

`itsupport@PersonalLab851.onmicrosoft.com`



\*\*Alias:\*\*

`helpdesk@PersonalLab851.onmicrosoft.com`



Both addresses route email to the same IT Support shared mailbox while the original IT Support address remains the primary SMTP address.



\## Mail Flow Test



Internal mail flow was tested using the Microsoft 365 lab accounts.



A test help desk request was sent from a user mailbox to the \*\*IT Support shared mailbox\*\*.



The IT Support mailbox was accessed using the delegated John Admin account, and the message was verified.



A response was then sent using the IT Support shared mailbox identity to demonstrate a basic help-desk email workflow.



\*\*Test workflow:\*\*



`Employee → IT Support Shared Mailbox → IT Administrator → Employee`



The test confirmed that the shared mailbox and delegated permissions were functioning as intended.



\## Tasks Completed



\* Accessed the Exchange Admin Center

\* Reviewed Exchange Online user mailboxes

\* Created the IT Support shared mailbox

\* Configured the shared mailbox email address

\* Granted John Admin Full Access permissions

\* Granted John Admin Send As permissions

\* Added a secondary `helpdesk` email alias

\* Reviewed mailbox properties and settings

\* Tested internal email delivery

\* Tested shared mailbox access

\* Tested sending email using the shared mailbox identity



\## Skills Demonstrated



\* Exchange Online administration

\* Exchange Admin Center navigation

\* User mailbox administration

\* Shared mailbox creation and management

\* Mailbox delegation

\* Full Access permissions

\* Send As permissions

\* SMTP email alias management

\* Internal mail flow testing

\* Microsoft Outlook administration

\* Microsoft 365 user and mailbox troubleshooting



\## Security Considerations



Administrative and authentication information was kept private throughout the lab.



\* No user passwords were stored in the GitHub repository.

\* No temporary passwords were included in screenshots.

\* No MFA authentication information or recovery codes were documented.

\* Mailbox permissions were assigned only to the account that required access.

\* The shared mailbox was used instead of sharing individual user credentials.

\* Administrative access followed the principle of limiting permissions to what was required for the lab.




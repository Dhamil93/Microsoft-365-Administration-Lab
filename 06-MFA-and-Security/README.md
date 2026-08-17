\# Microsoft 365 MFA \& Security Lab



\## Objective



The objective of this lab was to configure and test identity security controls in Microsoft Entra ID, including multifactor authentication (MFA), Security Defaults, Conditional Access, and user session management.



\## Environment



\* Microsoft 365 Business Premium

\* Microsoft Entra ID

\* Microsoft Entra Admin Center

\* Microsoft Authenticator

\* Microsoft 365 Admin Center

\* Tenant: `PersonalLab851.onmicrosoft.com`



\## Security Defaults



Security Defaults were reviewed within Microsoft Entra ID and confirmed to be enabled.



Security Defaults provide baseline identity protection for the Microsoft 365 tenant, including multifactor authentication requirements.



The existing Security Defaults configuration was left enabled during the lab.



\## MFA Registration



John Admin was used as the test account for MFA configuration.



Microsoft Authenticator was registered as an authentication method for the account.



After registration, Microsoft Entra ID confirmed that Microsoft Authenticator was available as a usable authentication method.



\## Conditional Access



A Conditional Access policy was created to demonstrate targeted MFA policy administration.



\*\*Policy name:\*\* `Require MFA - John Admin - Test`



\### Policy Configuration



\* User: John Admin

\* Target resources: All resources

\* Grant access: Require multifactor authentication

\* Policy state: Report-only



Report-only mode was used so the policy could be evaluated without immediately enforcing the configuration.



This provided a safe method of testing Conditional Access before production enforcement.



\## Conditional Access Testing



John Admin signed into Microsoft 365 after the Conditional Access policy was created.



The sign-in activity was reviewed through Microsoft Entra sign-in logs to examine how the Conditional Access policy evaluated the authentication attempt.



The policy remained in Report-only mode during testing.



\## Session Revocation



Existing sessions for John Admin were revoked through Microsoft Entra ID.



This exercise demonstrated an administrative response that can be used when:



\* A user reports a lost or stolen device

\* An account may have been compromised

\* Existing authentication sessions need to be invalidated

\* A user needs to be forced to authenticate again



\## Tasks Completed



\* Reviewed Microsoft Entra ID users

\* Reviewed user authentication methods

\* Verified Security Defaults

\* Registered Microsoft Authenticator

\* Verified MFA registration

\* Created a Conditional Access policy

\* Targeted a specific test user

\* Configured MFA as an access requirement

\* Used Report-only mode for safe policy testing

\* Reviewed sign-in activity

\* Revoked existing user sessions



\## Skills Demonstrated



\* Microsoft Entra ID administration

\* Multifactor authentication

\* Microsoft Authenticator

\* Identity and access management

\* Security Defaults

\* Conditional Access

\* Conditional Access policy testing

\* Authentication method administration

\* Sign-in monitoring

\* Session revocation

\* Microsoft 365 identity security



\## Security Considerations



\* Authentication secrets were not documented.

\* MFA QR codes were not stored or uploaded.

\* Temporary passwords were not included in the repository.

\* Authentication codes and recovery information were kept private.

\* Conditional Access was initially configured in Report-only mode to reduce the risk of accidental account lockout.

\* The primary administrator account was not used as the Conditional Access test account.

\* Security Defaults remained enabled during the lab.




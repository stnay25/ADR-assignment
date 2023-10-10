# ADR University network app

* Decision title: Integration with Active Directory

* Status: Accepted 

* Deciders: Stadium Nay

* Date: 2023-10-07

* Context and Problem Statement:
The objective is to integrate the university social networking app with the university's existing Active Directory for authentication. This integration is an important part of securing user data and ensuring appropriate access permission.  

* Considered Options:
[1] LDAP Integration
[2] Custom Authentication System
[3] Third-party Authentication Service
[4] OAuth 2.0 with Microsoft Authentication Library (MSAL)

* Decision:
The integration for the university app Active Directory will be OAuth 2.0 for authentication. User roles and permission will be managed by mapping Active Directory to app-specific roles. The MSAL integration will ensure smooth interaction with Active Directory.

* Rationale:
OAuth 2.0 has a secure authentication protocol that provides robust security for user authentication. This is well-suited for integration with enterprise systems like Active Directory.

MSAL simplified the integration process and ensured compatibility with Active Directory. By providing a reliable and well-documented framework for OAuth 2.0 authentication. 

Mapping the Active Directory groups to app-specific roles will enforce access control and ensure users have the appropriate permission within the app. 

Active Directory is a well-trusted and secure system for user management. This integration will improve app security and decrease the chances of unauthorized access. 

* Consequences:
There might be a learning curve, the development team may need to become proficient in OAuth 2.0 and MSAL if they aren’t familiar with it already. 

Compatibility with different Active Directory configurations and versions may require extra effort for testing and configuration. 

Regular updates and maintenance are necessary to ensure it’s compatible with evolving Active Directory and standards. 

* Follow-Up Action:
The team will implement OAuth 2.0 authentication with MSAL, this includes role mapping and access control mechanisms. 

Rigorous testing will be conducted to ensure compatibility with various Active Directory configurations. Any issues that are found will be addressed promptly. 

Documentation will be created to help guide the team on configuring, troubleshooting, and maintaining the Active Directory integration.

Regular security audit testing will be conducted to verify the security of integration and address any vulnerabilities. 

This action will ensure a secure and efficient integration with Active Directory, which will enhance user data protection. 



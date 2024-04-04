# Application Security in Pega
Application security refers to the measures and practices put in place to protect software applications from security threats, vulnerabilities, and attacks throughout their entire lifecycle. It encompasses a range of techniques, tools, and processes designed to identify, mitigate, and prevent security risks that could compromise the confidentiality, integrity, or availability of an application and its data.

## Critical Security Areas
### Data Encryption
Data Encryption protects sensitive data within your application without affecting the functionality of Pega Platform™. You can select the encryption type used in your application to encrypt and decrypt passwords, properties, and BLOBs. Encrypted data easily complies with privacy policies, regulatory requirements, and contractual obligations for handling private data.
### Authentication
Authentication ensures that only users and systems whose identities have been verified can access your application. In Pega Platform, authentication includes user logins, platform requests to external services, and external service requests to the platform.
### Authorization
Authorization, also called access control, ensures that after logging in, a user only has access to the allowed platform features, interfaces, or data. 

Pega Platform offers three types of authorization: role-based access control (RBAC), attribute-based access control (ABAC), and client-based access control (CBAC). You can use authorization features individually or collectively to provide the strictest level of control.

**Note:**
While there exists some confusion between authentication and authorization, the difference is simple: *authentication* defines who can access the application (i.e. who can enter the door of your application) *authorization* defines what a specific user can do within the application (i.e. what actions are available to a user that has entered your application)
### Auditing
Auditing, also called accountability, is a systematic evaluation of the security of company information systems. Security is measured by how well it conforms to a set of established criteria.

Pega Platform tracks many types of security events such as failed logins and password changes. You can optionally track many other types of security events, as well as changes to rules and data. By tracking these changes, you can understand how your system is functioning and be alerted of any potential problems.

## Security Goals
Security is a shared responsibility between Pega and our clients. This common goal ensures the **AIC Triad** – availability, integrity, and confidentiality of your application.

### Availability
Availability prevents delays for authorized individuals when accessing systems or data. 
### Integrity
Integrity prevents unauthorized individuals from modifying systems or data.
### Confidentiality
Confidentiality prevents unauthorized individuals from accessing systems or data. 

## Security Checklist
The Security Checklist is a key feature of Pega Platform that assists clients in hardening their applications and systems. To assist in tracking the completion of the tasks in the checklist, Pega Platform automatically installs an application guideline Rule instance that includes the tasks in the Security Checklist for each version of your application.

Use the Security Checklist to prepare your application for deployment. By completing the tasks on this checklist, you can safeguard sensitive data and improve the security of your application.

Pega provides [Security Checklist Core Tasks](https://docs.pega.com/bundle/platform/page/platform/security/security-checklist-core-tasks.html) that are essential to accomplish to ensure your applicaion is secure. 

## Security Policies
### Application Level Security
Application-level security focuses on protecting the application from outsiders and unauthorized users. For example, with application-level security you:

* Reduce the risk of unauthorized users getting into or stealing data from your application
* Identify authorized users who need access to the application
* Create password and authentication policies

Application-level security considers all the ways you can protect the application, such as using third-party security tools or setting up multi-factor authentication. The goal of application-level security is to make it impossible for non-authorized users to break into, read, or otherwise access your application.

### Feature Security
Feature security
Feature security focuses on the application by determining the Case Types, features, and data that authorized users can or cannot access. For example, with feature security you:

* Set up security roles for Personas identified in each Case Type so that authorized users can access the application features they need
* Prevent users from viewing features or accessing data to which they should not have access
* Design role-based access control (RBAC), attribute-based access control (ABAC), and client-based access control (CBAC)
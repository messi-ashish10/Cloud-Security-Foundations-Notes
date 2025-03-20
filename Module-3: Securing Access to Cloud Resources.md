# AWS IAM and Access Management

## 1. Introduction to AWS IAM and Access Management
AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources. IAM allows you to manage access through users, groups, roles, and policies. IAM provides fine-grained control over who can access what resources and under which conditions.

### **Key Learning Objectives**
By the end of this module, you should be able to:
- Authorize access to AWS services using IAM users, groups, and roles.
- Differentiate between different types of security credentials in IAM.
- Implement identity-based and resource-based policies for secure access.
- Utilize additional AWS services for authentication and access management.
- Centrally manage policies for multiple AWS accounts.

---

## 2. IAM Fundamentals
### **What is IAM?**
- IAM is integrated into most AWS services, allowing centralized access control.
- Provides both **authentication** (verifying identity) and **authorization** (granting permissions).
- Supports multi-factor authentication (MFA) for enhanced security.
- Offers **identity federation** to allow users from corporate systems to access AWS resources.

### **IAM Components:**
- **IAM User:** Represents a person or application with long-term credentials.
- **IAM Group:** A collection of IAM users with shared permissions.
- **IAM Role:** Grants temporary credentials for a specific task or session.
- **IAM Policy:** A JSON document that defines permissions.

---

## 3. Authentication and Authorization
### **Authentication**
- Verifies the identity of the user or application.
- Uses credentials such as:
  - Username and password (for console access)
  - AWS access keys (for CLI or API access)
  - Multi-Factor Authentication (MFA)

### **Authorization**
- Determines what actions an authenticated user or application can perform.
- Uses policies to explicitly allow or deny actions on resources.

### **IAM Policies**
- Policies define what users or roles can do with AWS services.
- **Identity-Based Policies:** Attached to users, groups, or roles.
- **Resource-Based Policies:** Attached directly to AWS resources (like S3 buckets).
- **Permissions Boundaries:** Define the maximum permissions an entity can have.
- **AWS Organizations SCPs:** Set permission limits across multiple AWS accounts.
- **Access Control Lists (ACLs):** Control access to S3 buckets and objects.
- **Session Policies:** Used for temporary session permissions.

---

## 4. Multi-Factor Authentication (MFA)
- Adds an extra layer of security.
- Factors include:
  - Something you know (password)
  - Something you have (security token)
  - Something you are (biometric data)
- Common MFA devices: YubiKey, Google Authenticator, Authy.

---

## 5. IAM Roles and Temporary Credentials
- **Roles** allow services or users to assume permissions temporarily.
- **AWS Security Token Service (STS)** issues temporary security credentials.
- Roles are useful for cross-account access and service-to-service interactions.

### **Example Usage:**
1. Administrator creates an IAM role with S3 access.
2. An EC2 instance assumes the role to access the S3 bucket.
3. AWS STS provides temporary credentials.

---

## 6. AWS Organizations and Centralized Management
### **AWS Organizations:**
- Manage multiple AWS accounts from a central location.
- Implement **Service Control Policies (SCPs)** to control access at the organizational level.
- Structure accounts using **Organizational Units (OUs)** for better management.
- Support consolidated billing.

### **Best Practices:**
- Use AWS Organizations to simplify multi-account management.
- Apply SCPs to enforce security policies across all accounts.

---

## 7. Advanced IAM Features
### **IAM Managed Policies vs. Inline Policies**
- **Managed Policies:** Can be reused and attached to multiple entities.
- **Inline Policies:** Embedded directly within a single user, group, or role.
- **Best Practice:** Prefer managed policies over inline policies for scalability.

### **Evaluation Logic for IAM Policies**
- **Default Deny:** All requests are denied unless explicitly allowed.
- **Explicit Allow:** Overrides the default deny.
- **Explicit Deny:** Overrides any explicit allow.
- **Policy Evaluation Order:** All policies are evaluated before making a decision.

---

## 8. AWS Authentication Services
### **AWS Single Sign-On (SSO)**
- Unified administration to centrally manage user identities and access.
- Integrates with existing Active Directory and popular cloud applications.

### **AWS Directory Service**
- Managed Microsoft AD for directory-aware workloads.
- Facilitates seamless integration with existing AD environments.

### **Amazon Cognito**
- User authentication and authorization for web and mobile apps.
- Supports social identity providers (like Google and Facebook).

---

## 9. Best Practices for Secure Access
- Implement the **principle of least privilege**.
- Regularly audit and rotate credentials.
- Use MFA wherever possible.
- Enforce strong password policies.
- Enable **AWS CloudTrail** for auditing API calls.

---

## 10. Summary
AWS IAM provides robust access control and identity management through users, groups, roles, and policies. It integrates with various AWS services and allows fine-grained access control. By leveraging AWS Organizations and IAM best practices, you can secure your cloud infrastructure efficiently and effectively.

For more information, see:
- [IAM Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
- [AWS IAM User Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)
- [AWS Organizations User Guide](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_introduction.html)


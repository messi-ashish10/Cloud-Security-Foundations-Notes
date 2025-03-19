# AWS Cloud Security Governance and Managed Services

## 1. Introduction to Security and Governance in AWS
AWS security and governance can be managed by a centralized team known as a **Provisioning Team**, **Center of Excellence**, or **Managed Services Organization (MSO)**. These teams may be internal or external, with external vendors referred to as **Managed Service Providers (MSPs)**.

AWS validates AWS Partners under the **AWS Managed Service Provider (MSP) Program**. MSOs ensure security, compliance, and governance by establishing **repeatable processes and security guardrails** for cloud deployments.

## 2. Security in the AWS Cloud
### **Key Learning Objectives**
At the end of this module, you should be able to:
- Identify security features and benefits of cloud computing.
- Understand the security principles that AWS Cloud is structured around.
- Recognize which part of an application the user is responsible for securing in the cloud.

This module covers:
- **Security in the AWS Cloud**
- **Security Design Principles**
- **Shared Responsibility Model**
- Includes an **activity on the shared responsibility model** and a **knowledge check**.

## 3. Benefits of Cloud Computing
### **Key Advantages of Cloud Security:**
- **Trade fixed expense for variable expense**: Pay only for what you use instead of investing in data centers upfront.
- **Benefit from economies of scale**: Cloud providers aggregate customer usage, reducing costs.
- **On-demand capacity**: Scale infrastructure as needed, avoiding over-provisioning.
- **Increase speed and agility**: Deploy IT resources quickly, reducing time to market.
- **Stop spending on maintaining data centers**: Focus on core business instead of infrastructure management.
- **Go global in minutes**: Deploy applications worldwide for improved customer experience.

## 4. Security Principles: The CIA Triad
Security in AWS follows the **CIA triad**:
- **Confidentiality:** Ensuring only authorized users access information.
- **Integrity:** Maintaining data accuracy and trustworthiness.
- **Availability:** Ensuring data is accessible when needed.

Security in the cloud reduces **complexity and costs** compared to on-premises environments. AWS provides **software-based security tools** to monitor and protect resources.

## 5. Shared Responsibility Model
- **AWS is responsible for** securing the cloud infrastructure (physical, network, hypervisor security).
- **Customers are responsible for** securing everything they deploy **in** the cloud (data, applications, access control).
- **MSOs create security guardrails** for data protection, disaster recovery, and compliance.

## 6. Identity and Access Management (IAM)
AWS provides tools to manage **user authentication, roles, and access control**:
- **AWS IAM**: Securely control access to AWS resources.
- **AWS Security Token Service (STS)**: Temporary security credentials.
- **AWS CloudHSM**: Hardware security modules for encryption key management.
- **AWS CloudTrail**: Logs user activity and API calls for auditing.

## 7. Security Best Practices
### **Key Security Principles:**
- **Apply the principle of least privilege**: Restrict access to only those who need it.
- **Enable traceability**: Use monitoring and logging services.
- **Secure all layers**: Implement multi-layer security controls.
- **Automate security**: Utilize AWS security automation tools.
- **Protect data in transit and at rest**: Use encryption and access control.
- **Prepare for security events**: Develop incident response strategies.
- **Minimize the attack surface**: Reduce vulnerabilities and unnecessary access.

## 8. Compliance and Auditing
AWS provides compliance and monitoring tools to ensure regulatory adherence:
- **AWS Config**: Tracks configuration changes and compliance.
- **Amazon GuardDuty**: AI-powered threat detection.
- **AWS CloudTrail**: Audits API calls and security events.
- **AWS Security Hub**: Centralized security monitoring.

## 9. Summary
- AWS follows a **Shared Responsibility Model**.
- Organizations use **MSOs or MSPs** to enforce security best practices.
- AWS security leverages **software-based monitoring and protection tools**.
- **Customers must secure their cloud resources**, including security groups and data protection settings.

For more details, visit:
- **[AWS Managed Service Provider (MSP) Program](https://aws.amazon.com/partners/programs/msp/)**
- **[AWS Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)**
- **[What is Cloud Computing?](https://aws.amazon.com/what-is-cloud-computing/)**


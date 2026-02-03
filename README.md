## AWS EC2 Compute Baseline & Instance Management

Designed and validated an Amazon EC2 compute baseline with a focus on access control, instance management and operating system configuration. This project demonstrates how to deploy, operate and manage EC2 instances using AWS-native tooling and infrastructure best practices.

---

## Overview

This project demonstrates the deployment and operation of an Amazon EC2 instance using secure defaults, minimal access paths and managed administration. The focus is on reducing operational complexity, enforcing predictable access patterns and managing instances without reliance on public SSH or static credentials.

The implementation reflects common responsibilities in Cloud Engineer, Platform Engineer and Junior SRE roles, where compute instances must be manageable, auditable and easy to operate at scale.

---

## What I Built

- Amazon EC2 instance running Amazon Linux 2.
- IAM role with scoped permissions for Systems Manager–based management.
- Security Group allowing only required inbound traffic.
- Instance management via AWS Systems Manager Session Manager.
- Hardened OS configuration and system patching.
- System auditing enabled for operational visibility.
- Full resource cleanup after validation.

---

## Diagram

![Architecture Diagram](diagram.png)

---

## Implementation Highlights

- Launched an EC2 instance using controlled configuration and metadata settings.
- Attached an IAM role enabling SSM-based management without SSH keys.
- Restricted inbound traffic using Security Groups.
- Verified instance registration and access via Systems Manager.
- Applied OS configuration changes to standardize access behavior.
- Updated and patched the operating system.
- Enabled system auditing for traceability.
- Cleanly removed all resources after completion.

---

## Screenshots

Selected screenshots are included in the screenshots/ directory to validate instance configuration, access paths and system state.

---

## Key Takeaways

- EC2 instances should be operated through managed access paths, not direct SSH.
- IAM roles simplify credential management and reduce operational overhead.
- Security Groups act as the first layer of instance-level traffic control.
- OS configuration and patching are part of baseline compute ownership.
- Auditing improves visibility and supports troubleshooting and investigation.
- Clean teardown is essential for cost and environment hygiene.

---

## Relevance to Cloud & Platform Engineering

This project reflects real-world compute responsibilities:
- EC2 provisioning and configuration.
- IAM role–based instance access.
- Managed administration using AWS Systems Manager.
- OS baseline configuration.
- Operational visibility and lifecycle management.

--- 

## References

- [CIS Amazon Linux 2 Benchmark](https://www.cisecurity.org/benchmark/amazon_linux/)
- [AWS EC2 Security Best Practices](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-best-practices.html)
- [AWS Systems Manager Documentation](https://docs.aws.amazon.com/systems-manager/)

---

## Contact

Maintained by Sebastian Silva C. – Berlin, Germany
LinkedIn: https://www.linkedin.com/in/sebastiansilc

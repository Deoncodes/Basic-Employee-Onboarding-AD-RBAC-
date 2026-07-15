# Basic-Employee-Onboarding-AD-RBAC
Active Directory infrastructure rebuild for a fictional company called “Northstar Medical Group”. Includes domain setup, organisational structure, user provisioning, RBAC implementation, and incident resolution.

## Problem Statement
Northstar Medical Group fictional company,  they are fast growing currently experiencing difficulties with most of their processes. Their whole infrastructure/identity lifecycle workflow was previously outsourced to be managed by an MSP who did a very terrible job that has led to so many other issues. In the beginning this was fine but as the company grew much bigger this became a sore spot. The AD environment is completely disorganised, they had no RBAC policy in place, off-boarding and onboarding of employees was done manually with no sort of documentation for tracking or reference. This is healthcare and there were no audit trails, HIPAA is not a joke.

## Solution Overview
TThe solution was to take full ownership of the problem and overall architecture of NMG, started out by building a basic employee onboarding pipeline in AD. I Created OU's for each department in NMG and created Security-Groups with specific policies that varied according to each department. This would ensure there are no overlaps with permissions, access and ensure more security. Created a consistent digital identity for every employee in NMG and assigned attributes that would sync across all our systems, assigned access using RBAC enforcing principle of least privilege. This would ensure consistency, scalability and auditability. Made sure to create proper documentation of each process for reference and accurate bookkeeping.
I also simulated a mock ticket where a user was provisioned an incorrect level of access and resolved it.

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* CLI
* GitHub
* Group Policy

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Designed department-based OU structure (Finance, HR, IT, Operations)
* Implemented RBAC with security groups mapped to each department
* Provisioned 15 user accounts with consistent naming conventions and attribute standards
* Documented full incident resolution with root cause analysis
* Diagnosed and resolved a multi-cause access issue (wrong OU + missing group membership)

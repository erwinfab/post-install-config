<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>

# osTicket - Post-Install Configuration
*This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.*

### Executive Summary
This project focuses on the post-install configuration of the **osTicket** platform. I configured the system’s organizational hierarchy, including **Roles**, **Departments**, and **Teams**, and established **Service Level Agreements (SLAs)** to define ticket response and resolution expectations. This setup ensures a streamlined workflow for support agents and clear communication for end-users.

### Environments and Technologies Used
- **Microsoft Azure** (Virtual Machines/Compute)
- **Remote Desktop (RDP)**
- **Internet Information Services (IIS)**
- **osTicket Administration Panel**

### Operating Systems Used 
- *Windows 10* (21H2)

### Post-Install Configuration Objectives
* **User/Agent Differentiation**: Distinguishing between the Agent Panel and the Admin Panel.
* **Access Control**: Configuring grouping permissions and departmental visibility.
* **SLA Management**: Establishing response time targets for different ticket severities.
* **Help Topics**: Creating intuitive categories for users to streamline ticket routing.

## Configuration Steps

**Step 1**: **Configuring Roles, Departments, and Teams**

* To establish proper permissions, I created a **"Supreme Admin"** role within the Admin Panel. This role grants full administrative control over all ticket actions, including deletion and assignment.

  * I also configured the organizational structure by:

 1. **Departments**: Created a **SysAdmins** department to handle backend technical issues.
 2. **Teams**: Created an **"Online Banking"** team to group agents from different departments to work on specific high-priority business functions.

<img width="809" height="680" alt="image" src="https://github.com/user-attachments/assets/2359d275-94e8-4859-9486-302272dee139" />

---

**Step 2**: **Agent and User Provisioning**

* I configured the system to require **Registration**, ensuring that only authorized users can submit tickets. This enhances security and record-keeping.

I then provisioned new staff members to simulate a real-world help desk environment:
 * **Jane Doe**: Assigned to the **SysAdmins** department.
 * **John Doe**: Assigned to the **Support** department.
 * **Users**: Created profiles for **Karen** and **Ken** as the primary "customers" who will be generating support requests.

<img width="962" height="405" alt="image" src="https://github.com/user-attachments/assets/2b2ca5f0-7435-4845-a14e-f6f9012c2e54" />

---

**Step 3**: **Establishing SLAs and Help Topics**

To meet business requirements, I defined three **Service Level Agreements (SLAs)** to govern response times:
 * **Sev-A**: 1-hour grace period, 24/7 schedule (Critical Outages).
 * **Sev-B**: 4-hour grace period, 24/7 schedule (High Priority).
 * **Sev-C**: 8-hour grace period, Business Hours (Standard Requests).

Finally, I created several **Help Topics** (e.g., Password Reset, Equipment Request, Business Critical Outage). These topics allow the system to automatically route tickets to the correct department based on the user's selection.

<img width="885" height="344" alt="image" src="https://github.com/user-attachments/assets/fee25547-d252-4bd3-a199-f5faabf9907b" />

<img width="881" height="317" alt="image" src="https://github.com/user-attachments/assets/0b43a471-1997-4c02-a5fb-bf5d9b614949" />

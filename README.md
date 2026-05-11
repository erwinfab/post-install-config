<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>


# osTicket - Post-Install Configuration
*This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.*

## Executive Summary
This project focuses on the post-install configuration of the **osTicket** platform. I configured the system’s organizational hierarchy, including **Roles**, **Departments**, and **Teams**, and established **Service Level Agreements (SLAs)** to define ticket response and resolution expectations. This setup ensures a streamlined workflow for support agents and clear communication for end-users.

### Environments and Technologies Used

- **Microsoft Azure** (Virtual Machines/Compute)
- **Remote Desktop (RDP)**
- **Internet Information Services (IIS)**
- **osTicket Administration Panel**

### Operating Systems Used 

- Windows 10 (21H2)

### Post-Install Configuration Objectives

* **User/Agent Differentiation**: Distinguishing between the Agent Panel and the Admin Panel.

* **Access Control**: Configuring grouping permissions and departmental visibility.

* **SLA Management**: Establishing response time targets for different ticket severities.

* **Help Topics**: Creating intuitive categories for users to streamline ticket routing.

### Configuration Steps

**Step 1**: **Configuring Roles, Departments, and Teams**

* To establish proper permissions, I created a "Supreme Admin" role within the Admin Panel. This role grants full administrative control over all ticket actions, including deletion and assignment.

  * I also configured the organizational structure by:

1. **Departments**: Created a **SysAdmins** department to handle backend technical issues.

2. **Teams**: Created an **"Online Banking"** team to group agents from different departments to work on specific high-priority business functions.

<img width="809" height="680" alt="image" src="https://github.com/user-attachments/assets/2359d275-94e8-4859-9486-302272dee139" />

---



**Step 2**: **Agent and User Provisioning**


I configured the system to require **Registration**, ensuring that only authorized users can submit tickets. This enhances security and record-keeping.

I then provisioned new staff members to simulate a real-world help desk environment:

* **Jane Doe**: Assigned to the **SysAdmins** department.

* **John Doe**: Assigned to the **Support** department.

* **Users**: Created profiles for **Karen** and **Ken** as the primary "customers" who will be generating support requests.

<img width="961" height="427" alt="image" src="https://github.com/user-attachments/assets/34198790-18f2-4069-8fbf-96a77329917d" />

---


<h2>Step 3: Configure Agents (Staff)</h2>

With the structure in place, create your staff accounts. In the Admin Panel, go to Agents $\rightarrow$ Add New to create your two agents: "Jane" (assigned to the SysAdmins department/Online banking team) and "John" (assigned to the Support department).




<h2>Step 4: Configure Ticket Management Rules</h2>

The final step is to define the business rules for handling tickets. Go to Manage $\rightarrow$ SLA to create three service levels: "Sev-A" (1-hour grace period, 24/7), "Sev-B" (4-hour grace period, 24/7), and "Sev-C" (8-hour grace period, Business Hours)7. Lastly, navigate to Manage $\rightarrow$ Help Topics to create the ticket categories users will select, such as "Business Critical Outage," "Personal Computer Issues," "Equipment Request," and "Password Reset".


<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configuring Agent Roles to define staff permissions.
- Establishing Departments and Teams to organize agents and manage ticket visibility.
- Populating the system by creating Agents (staff) and Users (clients).
- Defining Service Level Agreements (SLAs) to set response time expectations.
- Building Help Topics to ensure proper ticket routing and data collection.
- Securing client access by requiring user registration to create tickets.

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Build the Organizational Structure (Roles, Departments & Teams)</h2>


First, the core business structure was built. I navigated to Admin Panel -> Agents -> Roles to create a "Supreme Admin" role with full permissions. Next, I set up ticket visibility and routing by creating Departments (Admin Panel -> Agents -> Departments), such as "SysAdmins." Finally, I configured Teams (Admin Panel -> Agents -> Teams) like "Online Banking" to allow for pulling agents from different departments onto a single team for specific issues.
</p>
<br />


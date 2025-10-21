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


<img width="407" height="294" alt="image" src="https://github.com/user-attachments/assets/f3806e64-5963-4c12-b1c1-e082bfc47e09" />
 <img width="399" height="255" alt="image" src="https://github.com/user-attachments/assets/899f311d-ae35-4f81-afb9-e118a55540b2" />
 <img width="407" height="360" alt="image" src="https://github.com/user-attachments/assets/90557095-42ab-4e4f-95e6-33a52f7aea44" />


</p>
<p>
<h2>Step 1: Configure Organizational Structure</h2>


First, set up the foundational structure for your agents. Navigate to Agents $\rightarrow$ Roles to create a "Supreme Admin" role. Then, define ticket routing and visibility by going to Agents $\rightarrow$ Departments and creating the "SysAdmins" department. Finally, go to Agents $\rightarrow$ Teams to create the "Online Banking" team, which lets you group agents from different departments for specific assignments
</p>
<br />

<img width="423" height="354" alt="image" src="https://github.com/user-attachments/assets/1fd330be-e7ae-45ca-87ba-188022bacf74" /> <img width="495" height="295" alt="image" src="https://github.com/user-attachments/assets/a19a990a-9e78-4095-8dac-9a9678047645" />



<h2>Step 2: Configure System Access & Users (Customers)</h2>

Next, secure the system and add your customers. Go to Settings $\rightarrow$ User Settings and uncheck "Allow anyone to create tickets" to ensure registration and login are required. After securing access, switch to the Agent Panel $\rightarrow$ Users $\rightarrow$ Add New to create the customer accounts "Karen" and "Ken".
</p>
<br />

<img width="414" height="528" alt="image" src="https://github.com/user-attachments/assets/be550c34-91fa-4dab-8cd5-ca2b8fe9d82f" /> <img width="384" height="525" alt="image" src="https://github.com/user-attachments/assets/cfe2a8f6-928d-46c8-a9e7-2a538a6f2a2b" />
<img width="410" height="279" alt="image" src="https://github.com/user-attachments/assets/2b3e5aaa-74d8-49cc-a11d-7b336cd9a8d7" /> <img width="397" height="271" alt="image" src="https://github.com/user-attachments/assets/e6747566-f3b0-4e66-91f4-f908a835672e" />



<h2>Step 3: Configure Agents (Staff)</h2>

With the structure in place, create your staff accounts. In the Admin Panel, go to Agents $\rightarrow$ Add New to create your two agents: "Jane" (assigned to the SysAdmins department/Online banking team) and "John" (assigned to the Support department).
</p>
<br />

<img width="472" height="352" alt="image" src="https://github.com/user-attachments/assets/2ce9d761-3b33-4e99-a6f8-43df35ffe140" /> <img width="469" height="332" alt="image" src="https://github.com/user-attachments/assets/bacfc5e6-74b3-468e-80dd-2ad5065510b5" />


<h2>Step 4: Configure Ticket Management Rules</h2>

The final step is to define the business rules for handling tickets. Go to Manage $\rightarrow$ SLA to create three service levels: "Sev-A" (1-hour grace period, 24/7), "Sev-B" (4-hour grace period, 24/7), and "Sev-C" (8-hour grace period, Business Hours)7. Lastly, navigate to Manage $\rightarrow$ Help Topics to create the ticket categories users will select, such as "Business Critical Outage," "Personal Computer Issues," "Equipment Request," and "Password Reset".
</p>
<br />

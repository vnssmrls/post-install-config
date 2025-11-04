<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop/Windows App
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Installation Configuration Objectives</h2>

  - Establish User Access and Roles
  - Organize Departments and Teams
  - Set User and Ticketing Rules
  - Define Service Level Agreements (SLAs)
  - Customize Help Topics for End Users



<h2>Configuration Steps</h2>
<p> You may access osTicket Admin/Analyst Panel:  
  <a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a></br> and End User Portal:  
  <a href="http://localhost/osTicket">http://localhost/osTicket</a><br>
 
<img src="https://i.imgur.com/hlBqe2I.png" height="80%" width="80%" alt="admin/end user"/>
</p>
<p>Acknowledge <b>Agent Panel</b> (for staff/admins) vs <b>Admin Panel</b> (for system configuration).</p>
<h3>Configure Roles (Grouping Permissions)</h3>

- Navigate to: Admin Panel → Agents → Roles  
- Create new role: Supreme Admin

<h3>Configure Departments (Ticket Visibility, HelpDesk vs SysAdmins vs Networking)</h3>

- Navigate to: Admin Panel → Agents → Departments  
- Create department: SysAdmins
  
<p>
<img src="https://i.imgur.com/UQj3jWd.png" height="80%" width="80%" alt="SysAdmins"/>
</p>

<h3>Configure Teams</h3>

- Navigate to: Admin Panel → Agents → Teams (pull agents from different departments)  
- Create team: Online Banking  

<h3>Allow Anyone To Create Tickets</h3>

- Navigate to: Admin Panel → Settings → User Settings  
- Uncheck: Unregistered users can create tickets  
- Enable: Registration Required (Require users to register and login to create tickets)

<h3>Configure Agents (Staff)</h3>

- Navigate to: Admin Panel → Agents → Add New  
  - Jane → Department: SysAdmins  
  - John → Department: Support 

<p>
<img src="https://i.imgur.com/KArKjIW.png" height="80%" width="80%" alt="Agents"/>
</p>

<h3>Configure Users (Customers)</h3>

- Navigate to: Agent Panel → Users → Add New  
  - Karen  
  - Ken  

<h3>Configure SLA (Service Level Agreements)</h3>

- Navigate to: Admin Panel → Manage → SLA  
  - Sev-A: Grace Period 1 hour, Schedule 24/7  
  - Sev-B: Grace Period 4 hours, Schedule 24/7  
  - Sev-C: Grace Period 8 hours, Schedule Business Hours  

<h3>Configure Help Topics</h3>

- Navigate to: Admin Panel → Manage → Help Topics  
  - Business Critical Outage  
  - Personal Computer Issues  
  - Equipment Request  
  - Password Reset  
  - Other

<p>
<img src="https://i.imgur.com/EJVhVTV.png" height="80%" width="80%" alt="Help Topics"/>
</p>

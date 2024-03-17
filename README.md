# osticket-config
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Configuration</h1>
This tutorial outlines the configuration of the open-source help desk ticketing system osTicket, within an Azure virtual machine environment.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>Configuration Steps</h2>

- Item 1: Create Roles for Agents 
- Item 2: Create Departments
- Item 3: Create Teams  
- Item 4: Allow Anyone to Create Tickets
- Item 5: Create New Accounts for Agents and Customers
- Item 6: Configure SLA
- Item 7: Create and Assign Help Topics

<h2><a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">Create Roles for Agents</a></h2>

<p>
<img src="https://i.imgur.com/WY36NGX.png" height="80%" width="80%" alt="Create Roles"/>
<img src="https://i.imgur.com/KUQurs6.png" height="80%" width="80%" alt="for Agents"/>
<img src="https://i.imgur.com/EptSBOB.png" height="80%" width="80%" alt="permissions"/>
</p>
<p>
To configure the osTicket system, first, access the Windows 10 virtual machine and log in. Then, within the osTicket platform, log in using administrator credentials. Navigate to the "Admin Panel," select "Agents," then "Roles," and proceed to create a new role named "Supreme Admin," granting it full permissions.
</p>
<br />

<h2><a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Create Departments</a></h2>

<p>
<img src="https://i.imgur.com/JmorWLF.png" height="80%" width="80%" alt="Departments"/>
</p>
<p>
After configuring roles, proceed to the "Departments" section within the osTicket admin panel. Create a top-level department titled "System Administrators". 
</p>
<br />

<h2><a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Create Teams</a></h2>

<p>
<img src="https://i.imgur.com/ZRlANVr.png" height="80%" width="80%" alt="Teams"/>
</p>
<p>
Following department setup, navigate to the "Teams" section in the osTicket admin panel. Create a team called "Level II Support" and include our account "user_admin" as a member.
</p>
<br />

<h2>Allow Anyone to Create Tickets</h2>

<p>
<img src="https://i.imgur.com/xmkHf90.png" height="80%" width="80%" alt="Allow"/>
</p>
<p>
Navigate to "Settings" and then "User Settings" within the osTicket admin panel. Ensure that the option "Require registration and login to create tickets" is unchecked, enabling anonymous ticket submission and allowing individuals to submit requests without the need for prior registration or login. 
</p>
<br />

<h2>Create New Accounts for <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Agents</a> and <a href="https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html">Customers</a></h2>

<p>
Within the admin panel navigate to "Agents" and select "Add New." Proceed to create two new agents, "Jane Doe" and "Joe Doe" (using their respective usernames: jane.doe and joe.doe), assigning them roles, departments, and teams as necessary for their responsibilities. These will be considered the "helpdesk employees". 
</p>

<p>
<img src="https://i.imgur.com/QdP6zy3.png" height="80%" width="80%" alt="New Accounts"/>
<img src="https://i.imgur.com/CfUrl78.png" height="80%" width="80%" alt="Agents"/>
<img src="https://i.imgur.com/xYYMYvt.png" height="80%" width="80%" alt="Add"/>
<img src="https://i.imgur.com/r1x4ZDN.png" height="80%" width="80%" alt="New"/>
</p>


<p>
Now navigate to the "Agent Panel" and access the "Users" section, then select "Add New" to create accounts for "Karen" and "Ken". These will be considered as the "customers". 
</p>

<p>
<img src="https://i.imgur.com/GXrSitA.png" height="80%" width="80%" alt="Agent Panel"/>
<img src="https://i.imgur.com/6l4GNpo.png" height="80%" width="80%" alt="Users"/>
<img src="https://i.imgur.com/AxPlsn7.png" height="80%" width="80%" alt="customers"/>
</p>

<br />

<h2><a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">Configure SLA</a></h2>

<p>
After returning to the "Admin Panel," navigate to "Manage" and then select "SLA." Proceed by choosing "Add New SLA Plan" to establish three distinct SLA plans: Sev-A, Sev-B, and Sev-C. These plans are designed to set expectations regarding ticket closure times for different severity levels. For Sev-A, set a 1-hour deadline, applicable 24/7. Sev-B extends the resolution time to 4 hours and is also available 24/7, while Sev-C allows for an 8-hour window, specifically during business hours. 
</p>

<p>
<img src="https://i.imgur.com/FCUX80f.png" height="80%" width="80%" alt="Configure SLA"/>
<img src="https://i.imgur.com/TMZSrHQ.png" height="80%" width="80%" alt="Configure"/>
<img src="https://i.imgur.com/5iFNDfI.png" height="80%" width="80%" alt="SLA"/>

</p>

<br />

<h2>Create and Assign Help Topics</h2>

<p>
<img src="https://i.imgur.com/zmu5Cns.png" height="80%" width="80%" alt="Create and Assign Help Topics"/>
</p>
<p>
Within the "Admin Panel" and "Manage" sections, navigate to "Help Topics" and proceed to create four distinct topics: Business Critical Outage, Personal Computer Issues, Equipment Required, and Password Reset. The purpose of creating these topics is to offer customers the ability to categorize their issues when submitting tickets. By presenting clear options, users can select the category that most accurately reflects their problem.  
</p>

<br />

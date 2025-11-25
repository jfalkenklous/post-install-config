<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles, Departments & Teams
- Configure Agents & Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img width="1705" height="948" alt="image" src="https://github.com/user-attachments/assets/d4064e67-18b7-4266-a410-b23b770a837e" />
</p>
<p>
Go to the Admin Panel of osTicket (http://localhost/osTicket/scp/login.php). Login with the Admin User you created from the osTicket: Prerequisites and Installation steps. Once logged in to the Admin Panel, navigate to Agents > Roles. Select Add New Role. Under the Definition tab, label the role as 'Supreme Admin'. Navigate to the Permissions tab and select all available permissions under the Ticket tab. Go to the Tasks tab and select all available tasks. Go to the Knowledgebase tab and select all available. Click Add Role. 
</p>
<br />

<p>
<img width="1123" height="474" alt="image" src="https://github.com/user-attachments/assets/b4c7972e-2ca5-4747-b15f-d9a35f29f372" />
</p>
<p>
Navigate to the Departments tab. Select Add New Department. Label it 'SysAdmins'. Scroll down and select 'Create Dept'. Delete the'Maintenance' department by selecting the box next to it, then selecting 'More' and select 'Delete'.  
</p>
<br />

<p>
<img width="1445" height="443" alt="image" src="https://github.com/user-attachments/assets/b0f012d5-df8d-4d5a-8eab-aace5054167a" />
</p>
<p>
Navigate to the Teams tab. Select Add New Team. Label it 'Online Banking'. Select 'Create Team'. 
</p>
<br />

<p>
<img width="1003" height="721" alt="image" src="https://github.com/user-attachments/assets/07b83f7b-ea50-4a2e-9fd3-a3b230a2bfde" />
</p>
<p>
Navigate to 'Settings' Go to 'Users'. Confirm the 'Registration Required' box is unchecked. 
</p>
<br />

<p>
<img width="1052" height="943" alt="image" src="https://github.com/user-attachments/assets/882fe350-a5b8-4438-84c6-482b1c0e3e5f" />
</p>
<p>
Navigate to the 'Agents' tab. Select 'Add New Agent'. Add Jane Doe. See screenshot above for information fields to enter for First Name, Last Name, Email Address, and Username. Navigate to the Access tab. Add Jane to the SysAdmins department with 'Supreme Admin' access. Navigate to the 'Teams' tab and add Jane to the 'Online Banking' team. Hit 'Create'.
</p>
<br />

<p>
<img width="1019" height="951" alt="image" src="https://github.com/user-attachments/assets/157784ce-51e1-4fad-b0b4-62f7449ab31f" />
</p>
<p>
Go back to the 'Agents' tab and select 'Add New Agent'. Add John Doe. See screenshot above for information fields to enter for First Name, Last Name, Email Address, and Username. Navigate to the Access tab. Add John to the Support department with 'All Access' access. Hit 'Create'.
</p>
<br />

<p>
<img width="790" height="468" alt="image" src="https://github.com/user-attachments/assets/8168f86d-6f44-4859-972b-c27a7a95777c" />
</p>
<p>
Navigate back to the 'Agents' tab. Select Jane Doe. Select 'Set Password'. De-select the 'Send the agent a password reset email' box. Type the new password as 'Password1', confirm the password, uncheck the 'Require password change at next logon' box and select 'Update'. Follow the same exact steps for John Doe. 
</p>
<br />

<p>
<img width="760" height="461" alt="image" src="https://github.com/user-attachments/assets/98e40494-9ee1-4713-8b46-857ba0e435d4" />
</p>
<p>
Navigate to the 'Agent Panel'. Select 'Users'. Select 'Add User'. Enter email address and name as shown in the above screenshot. Select 'Add User'.   
</p>
<br />

<p>
<img width="1035" height="538" alt="image" src="https://github.com/user-attachments/assets/e24d8474-c0d4-491c-ae6b-19852eac30db" />
</p>
<p>
Go back to the 'Admin Panel'. Select 'Manage'. Select 'SLA'. Select 'Add New SLA Plan'. Label the SLA Plan as 'Sev-A'. Enter the Grace Period as '1' (hour). For Schedule, select '24/7' and then hit 'Add Plan'. Now also, create Sev-B (Grace Period as '4', Schedule as '24/7). Then create Sev-C (Grace Period as '8', Schedule as 'Monday-Friday 8am -5pm with U.S. Holidays'). 
</p>
<br />

<p>
<img width="1106" height="719" alt="image" src="https://github.com/user-attachments/assets/69500929-ada2-46f1-8497-fdaadac76a53" />
</p>
<p>
Navigate to the 'Help Topics' tab. Select 'Add New Help Topic'. Label as 'Business Critical Outage' and select 'Report a Problem' under Parent Type. Select 'Add Topic'. Continue to create additional Help Topics for Personal Computer Issues, Equipment Reset, Password Reset, and Other - use your best judgement to add the topics under the appropriate parent type. 
</p>
<br />

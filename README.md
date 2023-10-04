# post-install-config

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

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure roles, departments,teams, and agents
- Give/change permissions 
- Create Service-level Agreements
- Add Help Topics

<h2>Configuration Steps</h2>


![LB2 Step 1](https://github.com/CGLuissi/post-install-config/assets/143234913/1229b350-eff9-4a0d-af53-4d79e29cf29f)

  
1.) We will begin this tutorial by configuring new roles inside our ticketing system. Agents inside of our help desk system are given permissions through the Roles assigned to them in a specific Department. The first role we will create is the Supreme Admin role, which has absolute authority and can do anything in our system. Start by going to the Admin Panel then clicking Agents, then Roles. Click Add New Role and name the role Supreme Admin. Click Permissions and check off every box within the Tickets, Task, and Knowledgebase fields. 
</p>
<br />

![LB2 Step 2](https://github.com/CGLuissi/post-install-config/assets/143234913/27dabc16-3194-4391-bc88-e7bbb5fb1731)


2.) In the Agents tab now, click on Departments and then Add New Department. Name this department System Administrators. This department will have our Supreme Admin and have complete control over our system. You may also play around with the other settings, but for now we are just going with the default options.
</p>
<br />

![LB2 Step 2 1](https://github.com/CGLuissi/post-install-config/assets/143234913/1366381a-7133-4baf-a37f-727a230facc0)

  
3.) Now we will create a new Team from the Agent panel. With Teams, you can organize and create groups of Agents with specific chracteristics. In our imaginary scenario, we are going to make a team consisting of level 2 support agents, but you can pretend to have a team of networking experts or whatever you'd like. Select Add New Team and then name the group Level 2 Support. In the Members tab, you can add yourself. 

![LB2 Stp3](https://github.com/CGLuissi/post-install-config/assets/143234913/4ed59388-8494-424d-8e21-c3bd998ec5eb)

4.) For this project, we're going to allow anyone to be able to create tickets, so head to the Admin Panel then click Settings, then User Settings. Scroll down and select Save Changes.

![LB2 4](https://github.com/CGLuissi/post-install-config/assets/143234913/2d277b23-1cca-4a06-87ce-69f4e8b86279)


5.) Now we are going to add Agents. Agents are the employees and members of our helpdesk teams that create, manage and resolve tickets. We are going to add 2 new agents, one as a member of Level 2 Support, and the other as a Supreme admin. Go to the Admin panel, then click Add New Agents. Fill out the details, and click set password, remembering to leave the 2 boxes unchecked. Next, go to Access and make the Level 2 Support Agent have Support as their primary department and All Access. The other account will have System Administrators as their primary department and their access will be Supreme Admin. This account will also have extended access to the Support department.

![LB2 5](https://github.com/CGLuissi/post-install-config/assets/143234913/f5cd7474-0379-44d7-8a0e-d260a45e8b35)


6.) Users of our ticketing system will also be needed, so we're going to create some too. In the Agent Panel, go to Users, then click Add User. Create two new users with any names. 

![LB 2 6](https://github.com/CGLuissi/post-install-config/assets/143234913/ade7874b-3bb1-4ff7-86fb-6d63dcb95463)


7.) We will also add Service-level Agreements. These indicate the priority of a given ticket and are added by users but can be changed or moved on the Agent side. Click Admin Panel then Manage then SLA. Create 3 new SLA Plans: Sev-A(1 day,24/7), Sev-B(4 hours,24/7), and SEV-C(8 hours, business hours). Users may be allowed to label a ticket as SEV-A, meaning that the issue is crucial and must be addressed within the hour at all times, but as an Agent you can drop the SLA level or take on the issue. 

![LB2 7](https://github.com/CGLuissi/post-install-config/assets/143234913/63abcec7-6e5b-4bef-a095-5a618d3df834)


8.) Finally, create a few new Help Topics. In the Manage tab, click Help Topics and Add New Help Topic. We can make a new topic named Business Critical Outage and another one titled Equipment Request. These two help topics are opposites in terms of severity, but are just some of the issues that may arise in an IT department. When tickets in these topics are made, we can evaluate them and assign them to other departments if need be.


</p>
<br />

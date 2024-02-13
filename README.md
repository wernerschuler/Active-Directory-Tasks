<h1>Active Directory Tickets</h1>

Create a user then assign that user admin privileges
--- 
- New --> User --> Enter the account information 

<img src="https://i.imgur.com/kqRxoQe.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

- Right click the user account --> Properties --> Member of --> Add --> type domain admins --> Check Names --> Apply --> OK
- Can see from the screenshot below this user now has admin privileges

<img src="https://i.imgur.com/SuazUl0.png" height="50%" width="50%" alt="creating a user in Active Directory"/>


How to check if a computer is being managed by Active Directory
--- 
- Right click Start --> System --> Rename is PC (advanced)
- Can see from the screenshot below that this PC is not being managed by Active Directory because it is in a workgroup

  <img src="https://i.imgur.com/BjD49pT.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

How to find information on the local account of a computer
-- 
- Right click Start --> Computer Management --> Local Users and Groups --> Users 

<img src="https://i.imgur.com/lwSSLT3.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

How to see which computer has been joined to the domain
--
- In the Domain Controller --> Domain name --> Computers

**Join a computer to the domain**
 - From the Azure Portal, set the computer's DNS settings to the DC’s Private IP address

<img src="https://i.imgur.com/uevDE61.png" height="50%" width="50%" alt="DNS settings in Azure"/>

- From the Azure Portal, restart the computer
- Login to the computer using the local admin credentials
- Right click Start --> System --> Rename this PC (advanced) --> Change --> Domain --> Enter your Domain name --> Enter the the Domain name\admin account & password

<img src="https://i.imgur.com/Ykohjyb.png" height="50%" width="50%" alt="DNS settings in Azure"/>

- Restart your computer
- Go to Active Directory Users and Computers and see if the computer has been added to the Computers folder

**When attemping to login using the account created in AD, the error message (screenshot below) appears**

<img src="https://i.imgur.com/6jJpbIC.png" height="50%" width="50%" alt="DNS settings in Azure"/>

- Server Manager --> Tools --> Group policy management -->

New Start from here 
---
<img src="https://i.imgur.com/SFbJrc3.png" height="50%" width="50%" alt="Adding a new staff member ticket"/>

- Right click New --> User --> Enter the user information
- Once user has been created --> Right click the account --> Properties --> Organisation --> Enter the Job Title --> General --> Enter the office number
- This user will now be able to login to any machine that is connected to the domain

<img src="https://i.imgur.com/OTJc1ww.png" height="50%" width="50%" alt="Ticket for creating a group and adding a user to that group"/>

- Right click --> New --> Group --> Enter the group name --> Enter the group type and scope
- Right click Stacey's name --> Properties --> Member of --> Add --> Type Marketing --> Check Names --> Apply --> OK

***Flashcard group type security & distribution, group scope - domain local, global, universe***
***Flashcard difference between organisational unit and containers***

<img src="https://i.imgur.com/AYHHp86.png" height="50%" width="50%" alt="Ticket for creating an organisational unit"/>

- Right click the domain name --> New --> Organisational Unit --> Enter the name
- Right click the Marketing group --> Move --> MarketingOU

**How to search for a user in AD**
- ADUC --> In the top bar select 'Find objects in active directory domain services' --> Enter the name of the user --> Find Now

**Do you know how to reset a password in AD**
- Find the user in AD --> Right click --> Reset password

**See password and lockout policy**
- AD --> Tools --> Group policy management --> Forest --> Domains --> Right click Default Domain policy --> Edit --> Policies --> Windows Settings --> Security settings --> Account policies

**Ticket: My account is locked can you help?**
- ***Just unlock the account***
- AD --> Right click the account --> Properties --> Account --> Unlock account

<img src="https://i.imgur.com/SuazUl0.png" height="50%" width="50%" alt="Ticket to disable an account"/>
- AD --> Right click the account --> Disable account







<h1>Active Directory Tickets</h1>

Purpose of Project
--
In this project I will be doing basic tasks in Active Directory. I will also download and use an Active Directory management and reporting software called ADManager Plus.

Tasks
--
**Create a user then assign that user admin privileges**
- New --> User --> Enter the account information 

<img src="https://i.imgur.com/kqRxoQe.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

- Right click the user account --> Properties --> Member of --> Add --> type domain admins --> Check Names --> Apply --> OK
- Can see from the screenshot below this user now has admin privileges

<img src="https://i.imgur.com/SuazUl0.png" height="50%" width="50%" alt="creating a user in Active Directory"/>


**How to check if a computer is being managed by Active Directory**
- Right click Start --> System --> Rename is PC (advanced)
- Can see from the screenshot below that this PC is not being managed by Active Directory because it is in a workgroup

  <img src="https://i.imgur.com/BjD49pT.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

**How to find information on the local account of a computer**
- Right click Start --> Computer Management --> Local Users and Groups --> Users 

<img src="https://i.imgur.com/lwSSLT3.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

**How to see which computer has been joined to the domain**
- In the Domain Controller --> Domain name --> Computers

**Join a computer to the domain**
- On the computer, set the DNS to be the DC's IP address
- Right click Start --> System --> Rename this PC (advanced) --> Change --> Domain --> Enter your Domain name --> Enter the the Domain name\admin account & passwo
- Go to Active Directory Users and Computers and see if the computer has been added to the Computers folder

  
**Ticket 1 <br>
Name: Charles Morgan <br>
Job title: HR Consultant <br>
Office: 349**

- Right click New --> User --> Enter the user information
- Once user has been created --> Right click the account --> Properties --> Organisation --> Enter the Job Title --> General --> Enter the office number

<img src="https://i.imgur.com/4BpGl1y.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

- This user will now be able to login to any machine that is connected to the domain

**Ticket 2 <br>
New Group <br>
Name: Human Resources <br>
Add Charles Morgan to this group** <br>

- Right click --> New --> Group --> Enter the group name --> Enter the group type and scope
- Right click the user's name --> Properties --> Member of --> Add --> Type Human Resources --> Check Names --> Apply --> OK

<img src="https://i.imgur.com/7sLKV8z.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

***Flashcard group type security & distribution, group scope - domain local, global, universe***
***Flashcard difference between organisational unit and containers***

**Ticket 3 <br>
New Organisational Unit <br>
OU: HumanResourceOU <br>
Add Human Resources group to OU**

- Right click the domain name --> New --> Organisational Unit --> Enter the name
- Right click the Human Resource group --> Move --> HumanResourcesOU

**How to search for a user in AD**
- ADUC --> In the top bar select 'Find objects in active directory domain services' --> Enter the name of the user --> Find Now

<img src="https://i.imgur.com/tqPqK61.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

**How to reset a password in AD**
- Find the user in AD --> Right click --> Reset password

**See password and lockout policy**
- AD --> Tools --> Group policy management --> Forest --> Domains --> Right click Default Domain policy --> Edit --> Policies --> Windows Settings --> Security settings --> Account policies

<img src="https://i.imgur.com/eT1BjFp.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

**Ticket 4:<br>
My account is locked can you help?**

- AD --> Right click the account --> Properties --> Account --> Unlock account
  
<img src="https://i.imgur.com/1tnmGj4.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

**How to disable an account**
- AD --> Right click the account --> Disable account

<br> <br>

**People may use scripts when they login**
 - Right click account --> Properties --> Profile
 - **Logon script** - script that is executed automatically when a user logs into their computer. Such as, run 
 a program, set up printers, and connect to shared folders.

**Home folder**
 - location on a network server where a user can store and access their personal files and data.
 - Right click account --> Properties --> Profile

**Changing someone's lastname can cause issues**
 - Their user account, email address, and other associated information may need to be updated to reflect the new last name.

**Get access to more features in the Properties tab**
- View --> Advanced Features

<img src="https://i.imgur.com/141ngkZ.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

**Download ADManager Plus**
 - **Note:** An application used to manage AD
 - Login to a computer with an admin account
 - If having problem connecting to the internet
   - Change adapter options --> Ethernet --> IPv4 --> Properties --> preferred dns: 8.8.8.8 (Change this back once download is complete)
 - Download google chrome
 - Search and downloadad manageengine admanager plus

<img src="https://i.imgur.com/8ynmxYf.png" height="50%" width="50%" alt="creating a user in Active Directory"/>

 - Once the download is complete, run the program as an administrator







<h1>Active Directory Tasks</h1>

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



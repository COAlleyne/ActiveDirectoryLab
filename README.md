<h1>Active Directory Home Lab</h1>


<h2>Description</h2>
In this project demonstration I am creating an Active Directory home lab environemnt using Oracle Virtual Box. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Oracle VirtualBox 7.0</b> 
- <b>Powershell</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Windows Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
Create VM: <br/>
<img src="https://i.imgur.com/mafK0b5.png" height="80%" width="80%"/>
<br />
<br />
Create Guest Additions:  <br/>
<img src="https://i.imgur.com/6NZWzW1.png" height="80%" width="80%"/>
<br />
<br />
Setup IP Adressing - NIC - Main Internet and NIC - VM Internet: <br/>
<img src="https://i.imgur.com/mmpA8IK.png" height="80%" width="80%"/>
<br />
<br />
Rename PC for clarity:  <br/>
<img src="https://i.imgur.com/hV27yZu.png" height="80%" width="80%"/>
<br />
<br />
Install Active Directory Domain Services - Select Server:  <br/>
<img src="https://i.imgur.com/908ZUmM.png" height="80%"/>
<br />
<br />
Server Roles:  <br/>
<img src="https://i.imgur.com/V5eRSUh.png" height="80%"/>
<br />
<br />
Install:  <br/>
<img src="https://i.imgur.com/V0FfP6Y.png" height="80%"/>
<br />
<br />
Promote to Domain:  <br/>
<img src="https://i.imgur.com/GjS8ekd.png" height="80%"/>
<br />
<br />
Add new forest:  <br/>
<img src="https://i.imgur.com/Zh3bB1z.png" height="80%"/>
<br />
<br />
Creating dedicated admin account:  <br/>
<img src="https://i.imgur.com/tGFWoIj.png" height="80%"/>
<br />
<br />
Creating the admin account within the new org:  <br/>
<img src="https://i.imgur.com/LU3zGtB.png" height="80%"/>
<br />
<br />
Creating the admin account within the new org continued:  <br/>
<img src="https://i.imgur.com/Ljm5GKN.png" height="80%"/>
<br />
<br />
Creating the admin account within the new org continued:  <br/>
<img src="https://i.imgur.com/QzSGuyj.png" height="80%"/>
<br />
<br />
Sign out in order to log back in under newly created admin account:  <br/>
<img src="https://i.imgur.com/qkbGCx3.png" height="80%"/>
<br />
<br />
Enabling access to internet through domain controller:  <br/>
<img src="https://i.imgur.com/tH9gAYm.png" height="80%"/>
<br />
<br />
Routing the support for NAT:  <br/>
<img src="hhttps://i.imgur.com/oXhuhmr.png" height="80%"/>
<br />
<br />
Allowing internal clients to connect to the internet:  <br/>
<img src="https://i.imgur.com/RDbectS.png" height="80%"/>
<br />
<br />
Choosing the correct NIC for internet access:  <br/>
<img src="https://i.imgur.com/l0IDVxU.png" height="80%"/>
<br />
<br />
Setting Up DHCP so internal clients can reach the external internet:  <br/>
<img src="https://i.imgur.com/BtMGp70.png" height="80%"/>
<br />
<br />
Setting Up DHCP scope to give out IP adresses to client computers:  <br/>
<img src="https://i.imgur.com/RG7My5d.png" height="80%"/>
<br />
<br />
Setting Up DHCP scope to give out IP adresses to client computers range of 100 addresses:  <br/>
<img src="https://i.imgur.com/wygh4k0.png" height="80%"/>
<br />
<br />
DHCP options - lease default 8 days per IP address:  <br/>
<img src="https://i.imgur.com/uoMphbI.png" height="80%"/>
<br />
<br />
Enter domain controller IP address:  <br/>
<img src="https://i.imgur.com/8FFkoAz.png" height="80%"/>
<br />
<br />
Finishing Range:  <br/>
<img src="https://i.imgur.com/orjTEjZ.png" height="80%"/>
<br />
<br />
Authorize domain server and refresh to bring online:  <br/>
<img src="https://i.imgur.com/pamrT8P.png" height="80%"/>
<br />
<br />
Result - IPv4 and IPv6 Online:  <br/>
<img src="https://i.imgur.com/xFBD5qp.png" height="80%"/>
<br />
<br />
Create client users with script:  <br/>
<img src="https://i.imgur.com/cjobpDb.png" height="80%"/>
<br />
<br />
Create client users - set execution policy to unrestricted for testing purposes avoiding needing digital signature:  <br/>
<img src="https://i.imgur.com/n3CcCF4.png" height="80%"/>
<br />
<br />
Users created - new users directory with all users listed:  <br/>
<img src="https://i.imgur.com/1gPih60.png" height="80%"/>
<br />
<br />
Create new VM to assign clients to it for testing purposes:  <br/>
<img src="https://i.imgur.com/iJfnUnM.png" height="80%"/>
<br />
<br />
Client VM using internal NAT emulating a corporate network:  <br/>
<img src="https://i.imgur.com/4O9ruOR.png" height="80%"/>
<br />
<br />
Confirm internet is working on client VM - checking default gateway and Google Ping to confirm:  <br/>
<img src="https://i.imgur.com/XInST0a.png" height="80%"/>
<br />
<br />
Joining client to domain:  <br/>
<img src="https://i.imgur.com/MA6txxF.png" height="80%"/>
<br />
<br />
Joining client to domain continued:  <br/>
<img src="https://i.imgur.com/AdHf5Ho.png" height="80%"/>
<br />
<br />
Displaying client VM with IP address lease on domain controller VM:  <br/>
<img src="https://i.imgur.com/1Ei9VHi.png" height="80%"/>
<br />
<br />
The active directory is now setup and ready to manage new client machines!  <br/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

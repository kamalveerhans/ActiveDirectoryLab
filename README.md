<h1>Active Directory Home Lab</h1>


<h2>Description</h2>
In this lab we're going to create an active directory home lab environment using Oracle Virtual Box. Configuring and running this lab will definately help develop my understanding of how active directory and windows networking works. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
Make a Domain controller virtual machine running server 19 ios: <br/>
<img src="https://i.imgur.com/k8UgMBm.png" height="80%" width="80%" 
<br />
<br />
Installed Active Directory and make our domain:  <br/>
<img src="https://i.imgur.com/W6lIuGx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configured RAS/NAT so the client on private network can reach the internet through domain controller:  <br/>
<img src="https://i.imgur.com/Ug7zB9d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup DHCP on the DC so when we create our windows 10 machine it can get an ip address: <br/>
<img src="https://i.imgur.com/mZ8gZIL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Ran a powershell script that automatically created 1000 users in Active Directory:  <br/>
<img src="https://i.imgur.com/YiIlZ80.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create another virtual machine and install windows 10 which is connected to private virtual box network:  <br/>
<img src="https://i.imgur.com/j8zwwbj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Name it client1 and join It to the domain and login into with one of our domain accounts:  <br/>
<img src="https://i.imgur.com/G6MyvJS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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

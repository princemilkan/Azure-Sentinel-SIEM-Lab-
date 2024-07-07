<h1>Wazuh SIEM Home lab configuration</h1>

<h2>Description</h2>
Project consists of a simple of creating VM and setting up and running Wazuh dashboard, installing wazuh agent and wazuh manager.
Analysing alerts<br/>
<br />
<h2>Platforms and Technology Used</h2>

- <b>Virtual Box </b>
- <b>Ubuntu Desktop 22.04</b>
- <b>Windows 10 client</b>


<h2>Lab walk-through:</h2>

<p align="center">
Created Domain Controler as DC with windows 19 Server ISO and Clinet PC with Windows 10 ISO in Virtual Box : <br/>
<img src="https://i.imgur.com/vSeAAEU.png" height="80%" width="80%" alt="VB"/>
<br />
<br />
2 Network Adapters (One for Internet another one is for internal connection)  <br/>
<img src="https://i.imgur.com/2GCtAhm.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Created Domain Controlar as DC and DNS <br/>
<img src="https://i.imgur.com/MY03Kft.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Craeted and configured  DHCP for mydomain.com<br/>
<img src="https://i.imgur.com/B3u5hEU.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Created Scope for other clinets and later connected by client 1<br/>
<img src="https://i.imgur.com/5dux4bz.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Created Organizational Unit _ADMINS and _USERS <br/>
<img src="https://i.imgur.com/0oJQG3I.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Created Admin account as a-mmilkan for Mahmudul Milkan <br/>
<img src="https://i.imgur.com/Yj3hcjv.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Created 1000+ users using Powershell script <br/>
<img src="https://i.imgur.com/YXFUYd3.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
List of users created <br/>
<img src="https://i.imgur.com/FsvrWdo.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Signing in using one of users from clinet 1 PC  <br/>
<img src="https://i.imgur.com/pKB4Cml.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Changed PC name to CLIENT1 and Assigned it to mydomain.com by using admin accounct  <br/>
<img src="https://i.imgur.com/wwhvBP1.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Netword adapter details of clinet1 <br/>
<img src="https://i.imgur.com/5nx2nK7.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Pinging from clinet1 pc  <br/>
<img src="https://i.imgur.com/Bjy6as3.png" height="80%" width="80%" alt="AD lab"/>
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

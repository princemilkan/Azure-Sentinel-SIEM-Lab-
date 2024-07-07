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
Virtual Box: Created two VM for thhis lab. Ubuntu 22.04 to set up Wazuh Manager and windows 10 client for Wazuh agent  <br/>
<img src="https://i.imgur.com/EnWObn4.png" height="80%" width="80%" alt="VB"/>
<br />
<br />
Instaling Wazuh manager on Ubuntu:
Specifications
RAM: 8GB+
HDD: 50GB+
OS: Ubuntu 22.04 LTS

Install Wazuh 4.7 with curl command as below.
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh && sudo bash ./wazuh-install.sh -a

Extract Wazuh Credentials
sudo tar -xvf wazuh-install-files.tar<br/>

<img src="https://i.imgur.com/VphMzTj.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Setting up Static IP for Wazuh server <br/>
<img src="https://i.imgur.com/49t7zpL.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Configuring the filebeat.yml file<br/>
<img src="https://i.imgur.com/rc8ypnr.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Configuring the ossec.conf file for wazuh manager <br/>
<img src="https://i.imgur.com/rc8ypnr.png" height="80%" width="80%" alt="AD lab"/>
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

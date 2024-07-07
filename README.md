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
Restarting Wazuh Manager <br/>
<img src="https://i.imgur.com/fQ87KfU.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Installing Sysmon on windows 10 client  <br/>
<img src="https://i.imgur.com/vmdw5v5.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
ossec.conf file for wazuh agent <br/>
<img src="https://i.imgur.com/POip8N1.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Collected Sysmon file name for ossec.cof file to add into <br/>
<img src="https://i.imgur.com/LsoAYXj.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Adding rules inside ossec.conf file. Deleted the highlighted part  <br/>
<img src="https://i.imgur.com/9qjhCOd.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Wazuh is up and running on ubuntu VM and windows 10 client has been added as Wazuh agent  <br/>
<img src="https://i.imgur.com/UzTe3Kb.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Created new index inside Wazuh dashboard <br/>
<img src="https://i.imgur.com/yg9CugT.png" height="80%" width="80%" alt="AD lab"/>
<br />
<br />
Getting alerts from windows 10 client machine <br/>
<img src="https://i.imgur.com/JJqSeS7.png" height="80%" width="80%" alt="AD lab"/>
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

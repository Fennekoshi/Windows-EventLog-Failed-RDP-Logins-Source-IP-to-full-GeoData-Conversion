# Windows-EventLog-Failed-RDP-Logins-Source-IP-to-full-GeoData-Conversion

<h2>Description</h2>
Project consists of a setup on Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. SIEM will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to look up the attackers Geolocation information and plot it on the Azure Sentinel Map!
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> 
- <b>Azure (Microsoft) Sentinel</b> 

<h2>Program walk-through:</h2>

<p align="center">
Create a Virtual Machine: <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000447926306349167/unknown.png?width=1438&height=676" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
Launch the utility: <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000447069498122362/unknown.png?width=1440&height=549" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
Turn off Windows Firewall on VM: <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000448657545511043/unknown.png?width=895&height=676" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run Script to get Geo location of attackers:  <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000201986236481636/unknown.png?width=909&height=676" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Custom Logs Workspace with Custom Fields from raw log:  <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000449283646042133/unknown.png?width=1050&height=676" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup map in sentinel with Latitude and Longitude (or country):  <br/>
<img src="https://cdn.discordapp.com/attachments/638804245650604032/1000450241855758386/unknown.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
First hour results:  <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000233101823332494/unknown.png?width=1185&height=676" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Final results after 18hrs:  <br/>
<img src="https://media.discordapp.net/attachments/638804245650604032/1000424302874730496/unknown.png?width=1195&height=676" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

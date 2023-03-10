<h1>Failed RDP to IP Geolocation Information</h1>


 ### [YouTube Demonstration (@16:20)](https://youtu.be/RoZeVbbZ0o0?t=980)
 - Credits to Josh Makador for the Idea & Tutorial

#

Microsoft Azure Resources: 
- 1 Virtual Machine
- Log Analytics Workspace Configurations added to the VM 
- Resource Group Configurations added to the VM

![AzureLabPic3](https://user-images.githubusercontent.com/127223469/223543049-27fd5ae7-6f83-4057-960b-c9a50f4123aa.png)

#

<h2>Description</h2>
<b>The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.
</b>
<br />
<br />
The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot.
We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to
look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

![AzureLab1](https://user-images.githubusercontent.com/127223469/223540691-87aca5c1-62c3-4ae0-913d-fb9a5b462ef3.png)


</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from Other Countries coming in; Custom logs being output with geodata</h2>

![PowerShellLabAzure1](https://user-images.githubusercontent.com/127223469/223541625-d610ff57-e981-46b8-9c50-fa2e7ae7abbb.png)


<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/krRFrK5.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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

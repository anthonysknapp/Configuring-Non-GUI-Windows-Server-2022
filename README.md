<h1>Configuring Windows 2022 Non-GUI<h1>

  <h2>Lab Objective </h2>
Understand the presentations needed for the creation of a working domain 

<h2>Description</h2>
Configuring Windows 2022 Server Core (Non-GUI ) to promote a domain controller 
<br />

<h2>Environments Used </h2>

- - <b>VirtualBox</b>
  - Windows Server 2022 Care
  - 
<h2>Lab Walk-through:</h2>

<p align="center">
Before launching the Virtual Machine, go into settings and choose the network tab. make sure the network is Attached to the Internal Network, 
Name intnet: <br/>
<img src="https://imgur.com/Xpm6lcD.png" height="80%" width="80%" alt="Configuring Windows Non-GUI Steps"/>
<br />
<br />
Launch the Virtual Machine and Login:  <br/>
<img src="https://imgur.com/Nh1s7Ob.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The virtual machine will launch into the sconfig window automatically: <br/>
<img src="https://imgur.com/6QLuj2s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter 2 to change the computer name and change the name to Server2, and then press enter; the system will ask if you would want to reboot; enter N for No:  <br/>
<img src="https://imgur.com/HyFWhn9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter 8 to go into the Network settings:  <br/>
<img src="https://imgur.com/OTpdEf8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter 1 to select the Available network adapters:  <br/>
<img src="https://imgur.com/MjoNXSO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Press 1 for Set Network Adapter Address, and then enter S for Static:  <br/>
<img src="https://imgur.com/Xv576F4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the Static Address as 10.0.0.2 and the subnet mask as 255.255.255.0, and leave the default gateway blank:  <br/>
<img src="https://imgur.com/MfSlVeC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go back to Network Settings and select the network adapter; press 2 to set the DNS Servers:  <br/>
<img src="https://imgur.com/b7B6Cir.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />
Enter new preferred DNS server 10.0.0.1, leave the alternate DNS as blank:  <br/>
<img src="https://imgur.com/q9dF8YW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />
Enter 15 to exit the power shell. in PowerShell turnoff firewall by entering "netsh advfirewall set allprofiles state off", and then reset the server by entering "Shutdown /r /t 30:  <br/>
<img src="https://imgur.com/nIV5gH1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<img src="https://imgur.com/8nnA5Oa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>   
</p>

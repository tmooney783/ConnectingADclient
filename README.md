<h1>Connecting a Windows 10 client to a Windows Server AD domain</h1>

<h2>In this project I learned the basics of using Active Directory to set up a DHCP and DNS server on Windows Server 2022 and connecting a Windows 10 client </h2>

<h2>Environments used:</h2>

- Oracle VirtualBox
- Windows Server 2022
- Windows 10

<h2>Project walk-through</h2>

<p align="center">
In 'Roles and Feastures', added Remote Access: <br/>
<img src="https://i.imgur.com/k6g9TeF.png" height="80%" width="80%"/>
<br />
<br />
Added Routing: <br/>
<img src="https://i.imgur.com/5bd3JxT.png" height="80%" width="80%"/>
<br />
<br />
Configured Routing and Remote Access: <br/>
<img src="https://i.imgur.com/8Do7PJV.png" height="80%" width="80%"/>
<br />
<br />
Enabled NAT: <br/>
<img src="https://i.imgur.com/Txo1Y2M.png" height="80%" width="80%"/>
<br />
<br />
Selected interface for internet access: <br/>
<img src="https://i.imgur.com/2RnYaCQ.png" height="80%" width="80%"/>
<br />
<br />
Installed DHCP: <br/>
<img src="https://i.imgur.com/8jcHNQE.png" height="80%" width="80%"/>
<br />
<br />
Set IP scope: <br/>
<img src="https://i.imgur.com/8W9134y.png" height="80%" width="80%"/>
<br />
<br />
Named scope: <br/>
<img src="https://i.imgur.com/CVDipUx.png" height="80%" width="80%"/>
<br />
<br />
Defined scope address range. I used a mask of /24: <br/>
<img src="https://i.imgur.com/nhQdeR6.png" height="80%" width="80%"/>
<br />
<br />
Set lease duration: <br/>
<img src="https://i.imgur.com/q1ptPO3.png" height="80%" width="80%"/>
<br />
<br />
Specified the domain controllers ip address to be used as a default gateway: <br/>
<img src="https://i.imgur.com/k7fsG8N.png" height="80%" width="80%"/>
<br />
<br />
Specified the domain controller as the DNS server: <br/>
<img src="https://i.imgur.com/a1njk4N.png" height="80%" width="80%"/>
<br />
<br />
When trying to add a win 10 client, it wasn't connecting to the domain to use the dhcp server, so I had to go
back and enable the router options under server options in the dhcp tool panel and specify this ip address: <br/>
<img src="https://i.imgur.com/22MY4Yo.png" height="80%" width="80%"/>
<br />
<br />
Renamed the Windows 10 client and joined it to the domain using an admin account: <br/>
<img src="https://i.imgur.com/RNuoANp.png" height="80%" width="80%"/>
<br />
<br />
</p>

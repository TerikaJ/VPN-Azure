<h1> Virtual Private Networks (VPN) 🛡️🔐 </h1> 

<img src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/e5433c45-2361-48de-9d7e-ef90a84a01d2" alt="VPN Diagram" width="600"/>

<h2> What is a Virtual Private Network (VPN)?</h2>

A Virtual Private Network (VPN) is a service that creates a secure, encrypted connection over a less secure network, such as the Internet. It allows users to send and receive data as if their devices were directly connected to a private network, ensuring privacy and security by masking the user's IP address and encrypting data traffic. VPNs protect sensitive information, maintain privacy, and access restricted or geo-blocked content. 

<img src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/271da2cf-f7ff-4a5c-8013-f461396c2a88" alt="VPN Diagram" width="275"/>

<br>
<br/>

<h2>Overview</h2>
In this tutorial, we will log into our virtual machine (VM), download and install the free version of Proton VPN, check and note our current IP address, activate the VPN in a new region, and then verify our new IP address.

<h3> Environments and Technologies Used: </h3>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop for MacOS
- Proton VPN (free)
- "What Is My IP Address"

<h3> Operating Systems Used: </h3>

-  MacOS
-  Windows 10

<h2> List of Prerequisites: </h2>

-  Azure Account/Subscription
-  Windows 10 VM ([Tutorial to create a VM](https://github.com/terikaj/azure-begin))

<h2> Instructions Overview: </h2>

**_You will need to have a VM already created for this project; if you don't already have one, follow my [tutorial](https://github.com/terikaj/azure-begin) to learn how to create one. For this project specifically, we'll want to create a VM in a region that is not native to ours._**
<img src="https://github.com/Kelsow96/VIrtual-Private-Networks/assets/169297569/55bfd30f-7630-4fde-ac26-96f5a6074b2e" alt="VPN Diagram" width="600"/>
<br>
<br/>

&nbsp;&nbsp;&nbsp;&nbsp;① Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within the VM and record the IP address.  
&nbsp;&nbsp;&nbsp;&nbsp;② Download and install Proton VPN (Free). If you don't already have an account, you must sign up.  
&nbsp;&nbsp;&nbsp;&nbsp;③ Open the VPN and choose a VPN server in another country.  
&nbsp;&nbsp;&nbsp;&nbsp;④ Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within the VM and record the new IP address.

<h3> Instructions: </h3>     

  1. Browse to https://whatismyipaddress.com/ within the VM and record the IP address. Our current IP address is 20.11.4.178
![image](https://github.com/Kelsow96/VIrtual-Private-Networks/assets/169297569/51fa5616-aad3-4266-b9a2-371253f03362)
<br>
<br/>

  2. Download and Install Proton VPN (Free). If you don't already have an account, you must sign up.  
![image](https://github.com/Kelsow96/VIrtual-Private-Networks/assets/169297569/77184235-93eb-43e6-b9be-31425f7c3db4)
<br>
<br/>

  3. Open Proton VPN, log in with your account, and select "Fastest" connection. We have to use "Fastest" connection because we have a free account. If you pay for the upgraded versions of Proton VPN, you can select any country you'd like!
![image](https://github.com/Kelsow96/VIrtual-Private-Networks/assets/169297569/99b1c46f-294f-4efe-bfb9-a40fe70d134a)
![Capture](https://github.com/Kelsow96/VIrtual-Private-Networks/assets/169297569/8b1e8000-7f38-4850-ba19-efe4f89b4fb6)
<br>
<br/>

  4. Browse back to https://whatismyipaddress.com/ and record the new IP address. Our new IP address is 37.19.200.2. Our VM's public IP address (the one assigned by Azure) is now being masked by our new VPN IP address (37.19.200.2). So, any web traffic will now be routed through the new IP address VPN server, encrypting and protecting our web data. 
![image](https://github.com/Kelsow96/VIrtual-Private-Networks/assets/169297569/08d92b1a-960c-4d06-baf2-b7340583b369)
<br>
<br/>

<h2> Summary </h2>

- In conclusion, we successfully logged into our virtual machine (VM), downloaded and installed Proton VPN (free version), noted our current IP address, activated the VPN in a new region and confirmed our new IP address. This process demonstrates how to effectively use a VPN to change your IP location for added security and privacy.

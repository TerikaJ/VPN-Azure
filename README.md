<h1> Virtual Private Networks (VPN) 🛡️🔐 </h1> 

<img src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/e5433c45-2361-48de-9d7e-ef90a84a01d2" alt="VPN Diagram" width="600"/>

<h2> What is a Virtual Private Network (VPN)?</h2>

A Virtual Private Network (VPN) creates a secure, encrypted connection over an insecure network, like the Internet. It allows users to send and receive data as if connected to a private network, ensuring privacy and security by masking IP addresses and encrypting data traffic. VPNs protect sensitive information, maintain privacy, and provide access to restricted or geo-blocked content.


<img src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/271da2cf-f7ff-4a5c-8013-f461396c2a88" alt="VPN Diagram" width="275"/>

<br>
<br/>

<h1>Overview</h1>
In this tutorial, we will log into our virtual machine (VM), download and install the free version of Proton VPN, check and note our current IP address, activate the VPN in a new region, and then verify our new IP address.

<h3> Environments and Technologies Used: </h3>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop for MacOS
- Proton VPN (free)
- "What Is My IP Address"

<h3> Operating Systems Used: </h3>

-  MacOS
-  Windows 10

<h3> List of Prerequisites: </h3>

-  Azure Account/Subscription
-  Windows 10 VM ([Tutorial to create a VM](https://github.com/terikaj/azure-begin))

<h2> Instructions: </h2>

① Navigate to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within your home computer and record the IPv4 address. This will give you more context into how exactly the tunnel works within the VM and your VPN. We're ultimately creating 2 VPNs: one from our home computer into the virtual machine, and one from the virtual machine into Proton VPN. 

#### Current IP address for Home Computer is 104.14.134.35
#### City: Hayward

<img width="550" alt="1  IP (Home Computer)" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/cac0d689-cd06-49ff-81ff-c1f4a555bcfa">

***Important: You should already have a VM already created for this project; if you don't already have one, follow this [tutorial](https://github.com/terikaj/azure-begin) to create one. For this project specifically, we'll want to create a VM in a region that is not native to ours. In this example we use: South Africa***


<img width="550" alt="4  VM Set-Up" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/ac668cb6-dcd1-41d7-ba62-fc43cd3a6388">

<br>
<br/>   

② Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within the VM and record the IP address. 
#### Current IP address for VM is 102.37.221.63
#### City: Johannesburg
<img width="550" alt="7  IP (VM)" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/05db2dea-ec65-42f0-ad9e-ea0322d131b0">

<br>
<br/>

③ Download and install Proton VPN (Free). Please ensure that you sign up for an account.  
<img width="550" alt="8  Proton for Windows (Download)" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/c118cadd-c745-4c85-950e-7cf1579c5c77">

<br>
<br/>

④ Open the VPN, log in with your account, and select "Fastest" connection. "Fastest" connection is required for a free account. The upgraded version allows the selection of any country!  
<img width="550" alt="9  Sign into Proton" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/769fd422-3798-42c4-9551-6d3d4cd10f83">
<img width="550" alt="10  Select Fastest and Connect" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/2e8062ec-aad4-48a0-9c0a-7a286f2d6be0">

<br>
<br/>

&#9316; Browse back to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within the VM and record the new IP address. 

#### New IP address for VM is 89.39.107.198 
#### City: Darad Kola

Our VM's public IP address (the one assigned by Azure) is now being masked by our new VPN IP address (37.19.200.2). So, any web traffic will now be routed through the new IP address VPN server, encrypting and protecting our web data.  
<img width="550" alt="11  IP (VPN)" src="https://github.com/TerikaJ/VPN-Azure/assets/136477450/0b940e57-7904-45b1-9c87-9919a3eb511b">

<br>
<br/>

<h2> Conclusion </h2>

In conclusion, we logged into our virtual machine (VM), installed Proton VPN (free version), noted our current IP address, activated the VPN in a new region, and confirmed our new IP address. This process demonstrates how to use a VPN to change your IP location for added security and privacy.

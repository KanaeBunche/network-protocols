<p align="center">
  <img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Testing VPN Connection and IP Location with Azure Virtual Machines</h1>
This tutorial covers testing the IP address on a local machine, checking the IP location on a Virtual Machine (VM) without a VPN, and testing the IP location with a VPN on the local machine.

<h2>Environments and Technologies Used</h2>

- **Microsoft Azure (Virtual Machines/Compute)**
- **Remote Desktop (RDP)**
- **ProtonVPN (Free Plan)**
- **Browser (for testing IP location)**
- **WhatIsMyIPAddress (IP address checker)**

<h2>Operating Systems Used</h2>

- **Windows 10 (VM on Azure)**
- **Local Machine (for VPN setup)**

<h2>High-Level Steps</h2>

1. **Check Local Machine’s IP Address**  
   Open a browser on the local machine and go to [WhatIsMyIPAddress](https://whatismyipaddress.com/). Note the IP address displayed.

2. **Test IP Location Without VPN on Virtual Machine**  
   Log into a Virtual Machine (VM) on Azure. Open a browser and visit [WhatIsMyIPAddress](https://whatismyipaddress.com/) to check the IP address.

   [![Watch the video on Testing IP Location Without VPN](https://img.youtube.com/vi/YFNkjJf3lo8/0.jpg)](https://www.youtube.com/watch?v=YFNkjJf3lo8)

   *Click the image or [here](https://www.youtube.com/watch?v=YFNkjJf3lo8) to watch a video demo.*


3. **Test IP Location With VPN on Virtual Machine**  
   Install ProtonVPN on the virtual machine. Connect to a VPN server in a different country (e.g., Japan). Visit [WhatIsMyIPAddress](https://whatismyipaddress.com/) and note the new IP address.

   [![Watch the video on Testing IP Location With VPN](https://img.youtube.com/vi/zyeGKbw1tGI/0.jpg)](https://www.youtube.com/watch?v=zyeGKbw1tGI)

   *Click the image or [here](https://www.youtube.com/watch?v=zyeGKbw1tGI) to watch a video demo.*

4. **Clean Up Azure Resources**  
   Delete the resource group containing the VM in Azure to avoid unnecessary charges.

   <p align="center">
     <img src="https://i.ibb.co/8mg1jKj/Screenshot-2024-11-29-at-11-18-49-PM.png" alt="Clean Up Resources"/>
   </p>

<h2>Actions and Observations</h2>

<p>
  The local machine’s IP address shows the actual location. The VM’s IP address reflects the region of the VM. With ProtonVPN enabled, the local machine’s IP address will show the location of the VPN server (e.g., Japan).
</p>

<h2>Conclusion</h2>
This demonstration illustrates how VPNs alter IP addresses and their impact on network security.

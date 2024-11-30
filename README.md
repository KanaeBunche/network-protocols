<p align="center">
  <img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Testing VPN Connection and IP Location with Azure Virtual Machines</h1>
In this tutorial, we will walk through the process of testing your local machine’s IP address, checking the IP location on a Virtual Machine (VM) without a VPN, and then testing the IP location with a VPN on your local machine.

<h2>Video Demonstration</h2>

- ### [YouTube: VPN Connection and IP Location Testing](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- **Microsoft Azure (Virtual Machines/Compute)**
- **Remote Desktop (RDP)**
- **ProtonVPN (Free Plan)**
- **Browser (for testing IP location)**
- **WhatIsMyIPAddress (IP address checker)**

<h2>Operating Systems Used</h2>

- **Windows 10 (VM on Azure)**
- **Your Local Machine (for VPN setup)**

<h2>High-Level Steps</h2>

1. **Check Your Local Machine’s IP Address**  
   Open a browser on your local machine and go to [WhatIsMyIPAddress](https://whatismyipaddress.com/). Note down the IP address displayed.

   <p align="center">
     <img src="https://i.ibb.co/r7j9Y4p/Screenshot-2024-11-29-at-10-53-16-PM.png" alt="Check Local IP Address"/>
   </p>
   
2. **Test IP Location Without VPN on Virtual Machine**  
   Create and log into a Virtual Machine (VM) in Azure. Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within your VM and take note of the IP address.
   
   <p align="center">
     <img src="https://s2.ezgif.com/tmp/ezgif-2-4780c7db44.gif" alt="Check VM IP Without VPN"/>
   </p>

3. **Test IP Location With VPN on Virtual Machine**  
   Sign up for ProtonVPN and install the client on your local machine. Choose a server in a different country (e.g., Japan) and connect to the VPN. Visit [WhatIsMyIPAddress](https://whatismyipaddress.com/) again and note down the new IP address.

   <p align="center">
     <img src="https://s6.ezgif.com/tmp/ezgif-6-435001c9d8.gif" alt="Check IP with VPN on Local Machine"/>
   </p>

4. **Clean Up Azure Resources**  
   After testing, return to your Azure portal and delete the resource group containing the VM. Ensure the resources are properly removed to avoid unnecessary charges.

   <p align="center">
     <img src="https://i.imgur.com/example.gif" alt="Clean Up Resources"/>
   </p>

<h2>Actions and Observations</h2>

<p>
  After checking your local machine’s IP address, you will notice it reflects your actual geographical location. On the VM, the IP address will be from the country of the VM’s region. When you enable ProtonVPN on your local machine, the IP address will change to the location of the selected server (e.g., Japan), and websites will display content based on that location.
</p>

<h2>Conclusion</h2>
Through this exercise, you can better understand how VPNs alter your location online and the significance of IP address tracking in network security.

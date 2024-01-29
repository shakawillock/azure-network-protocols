<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a resource group in Azure
- Create a Windows VM and a Linux VM
- Use Remote Desktop to connect to Windows VM
- Install Wireshark in Windows VM
- Filter by ICMP traffic in Windows VM
- Ping the private IP address of Linux VM from Windows VM
- In Windows VM, open Powershell, ping a public address, and observe traffic in Wireshark
- Initiate non-stop ping from Windows VM to Linux VM
- Open the Network Security Group that Linux VM is using and disable ICMP traffic
- Observe ICMP traffic in Wireshark
- Re-enable ICMP traffic
- Observe ICMP traffic in Wireshark again
- Filter for SSH traffic in Wireshark
- Type commands into Linux VM and observe the SSH traffic in Wireshark
- Filter for DHCP traffic in Wireshark
- Issue a new IP address in Windows VM from the command line
- Observe DHCP traffic in Wireshark
- Filter for DNS traffic in Wireshark
- Use nslookup in command line to find what the IP addresses are for a few public websites
- Observe DNS traffic in Wireshark
- Filter for RDP traffic in Wireshark
- Observe the non-stop spam of traffic
- Close Remote Desktop and delete the resource groups/VMs

<h2>Actions and Observations</h2>

<p>1. Create a resource group in Azure </p>

<p>2. Create a Windows VM and a Linux VM </p>
<p>
<img src="https://i.imgur.com/hQlRW3d.png" height="80%" width="80%" alt="Azure Virtual Machines"/>
</p>
<br />

<p>3. Use remote Remote Desktop to connect to Windows VM </p>

<p>4. Install Wireshark in Windows VM </p>
<p>
<img src="https://i.imgur.com/tjceTNI.png" height="80%" width="80%" alt="Wireshark"/>
</p>
<br />

<p>5. Filter by ICMP traffic in Windows VM </p>

<p>
<img src="https://i.imgur.com/cv2CAgu.png" height="80%" width="80%" alt="Wireshark IMCP Traffic"/>
</p>
<br />

<p>6. Ping the private IP address of Linux VM from Windows VM </p>

<p>
<img src="https://i.imgur.com/DiQ3gfI.png" height="80%" width="80%" alt="Wireshark Ping Traffic"/>
</p>
<br />

<p>7. In Windows VM, open Powershell, ping a public address, and observe traffic in Wireshark </p>

<p>
<img src="https://i.imgur.com/fNvBiON.png" height="80%" width="80%" alt="Wireshark Ping Public Address"/>
</p>
<br />

<p>8. Initiate non-stop ping from Windows VM to Linux VM</p>
<p>
<img src="https://i.imgur.com/jWxQNb5.png" height="80%" width="80%" alt="Wireshark Non Stop Ping"/>
</p>
<br />

<p>9. Open the Network Security Group that Linux VM is using and disable ICMP traffic </p>
<p>
<img src="https://i.imgur.com/Z818WTP.png" height="80%" width="80%" alt="Network Security Group"/>
</p>
<br />

<p>10. Observe ICMP traffic in Wireshark </p>
<p>
<img src="https://i.imgur.com/mlMbWD8.png" height="80%" width="80%" alt="Wireshark Ping Public Address"/>
</p>
<br />

<p>11. Re-enable ICMP traffic </p>

<p>12. Observe ICMP traffic in Wireshark again </p>

<p>13. Filter for SSH traffic in Wireshark </p>
<p>
<img src="https://i.imgur.com/LqW4vcf.png" height="80%" width="80%" alt="Wireshark SSH"/>
</p>
<br />

<p>14. Type commands into Linux VM and observe the SSH traffic in Wireshark </p>
<p>
<img src="https://i.imgur.com/gd3BItl.png" height="80%" width="80%" alt="Wireshark SSH"/>
</p>
<br />


<p>15. Filter for DHCP traffic in Wireshark </p>
<p>
<img src="https://i.imgur.com/ncbjFFR.png" height="80%" width="80%" alt="Wireshark DHCP"/>
</p>
<br />

<p>16. Issue a new IP address in Windows VM from the command line </p>

<p>17. Observe DHCP traffic in Wireshark </p>
<p>
<img src="https://i.imgur.com/9y30f2i.png" height="80%" width="80%" alt="Wireshark SSH"/>
</p>
<br />

<p>18. Filter for DNS traffic in Wireshark </p>
<p>
<img src="https://i.imgur.com/hllEYVs.png" height="80%" width="80%" alt="Wireshark DNS"/>
</p>
<br />

<p>19. Observe DNS traffic in Wireshark </p>

<p>20. Filter for RDP traffic in Wireshark</p>
<p>
<img src="https://i.imgur.com/YbN5HAK.png" height="80%" width="80%" alt="Wireshark RDP"/>
</p>
<br />

<p>21. Observe the non-stop spam of traffic </p>

<p>22. Close Remote Desktop and delete the resource groups/VMs </p>

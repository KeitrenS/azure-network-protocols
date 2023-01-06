<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, DHCP, DNS, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Download Wireshark Protocol Analyzer
- Generate Traffic with ICMP protocol
- Configure a Network Firewall
- Renew IP with DHCP protocol
- Observe Traffic with DNS protocol

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/sIdory5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Go to Wireshark.org and download and install the Protocol Analyzer Wireshark.
</p>
<br />

<p>
<img src="https://i.imgur.com/Na5iRpp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once installed type in the protocol ICMP in the search engine to filter for raw ICMP data traffic.
</p>
<br />

<p>

</p>
<p>
 A firewall is setup in Azure to block ICMP traffic flow from VM1 to VM2.
</p>
<br />

<p>
<img src="https://i.imgur.com/Smi7GP4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After restoring and allowing traffic to resume from VM1 to VM2, renew the IP address by typing in DHCP protocol 'ipconfig /renew' in the command line.
</p>
<br />

<p>
<img src="https://i.imgur.com/oicSi2B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
With the command line 'nslookup' typed in, observe the domain configuration of various IP address.
</p>
<br />

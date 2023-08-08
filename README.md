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

- Create 2 Virtual Machines in Microsoft Azure
    - 1 Windows 10 (21H2) Machine
    - 1 Ubuntu Server 20.04
- Using Remote Desktop Sign into Windows 10 Machine
- Download Wireshark


<h2>Virtual Machines</h2>

<p>

![Screenshot 2023-08-07 192857](https://github.com/ryanhuntercarline/azure-network-protocols/assets/141659465/045e4f9d-a622-4003-ac1e-8c0372b376db)

</p>
<p>
 By utilizing separate virtual machines, you can create a controlled environment where you have full control over network configurations, firewall rules, and security settings. This isolation ensures that the network traffic you're analyzing is focused solely on the communication between the two designated IP addresses
</p>
<br />

<h2>Remote Desktop</h2>

<p>

![Screenshot 2023-08-07 193311](https://github.com/ryanhuntercarline/azure-network-protocols/assets/141659465/1b2bb876-ed93-4250-a183-912758531279)![Screenshot 2023-08-07 193434](https://github.com/ryanhuntercarline/azure-network-protocols/assets/141659465/d142eaf9-5027-41e6-9ed9-351800fafb02)

</p>
<p>
Using Remote Desktop, you can access the Windows 10 virtual machine (VM-1). Copy the public IP Address of VM-1, as demonstrated above, and paste it into Remote Desktop. After signing in with the provided username and password, you'll gain entry to VM-1
</p>
<br />

<h2>Wireshark</h2>

<p>

  ![Screenshot 2023-08-07 194011](https://github.com/ryanhuntercarline/azure-network-protocols/assets/141659465/0e5ccc34-4035-446b-bd1c-0220f2f46d2f)

</p>
<p>
Wireshark is a widely used open-source network protocol analyzer that captures and inspects data packets traveling over a computer network. It allows users to examine network traffic, diagnose issues, and analyze communication patterns for troubleshooting and security purposes

Once you have downloaded Wireshark to the Windows 10 VM you will be able to observe traffic within the Windows 10 VM as well as traffic between the two VMs you have created

Use Wireshark to search for and view the different network protocols (SSH, RDH, DNS, HTTP/S, ICMP)  
</p>
<br />

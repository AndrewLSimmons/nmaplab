# How to Scan a Host using the Nmap Utility in Kali Linux? 
<h2>Description</h2>
The Network Mapper (Nmap) utility is a common tool used with hackers as well as system administrators to scan a network host or device such as a server, pc, router, etc. The goal of the Nmap utility is to gather information about a targeted system or network. <br /><br />
The information that will be gathered in the Nmap lab includes:<br /><br />
<li>Open ports</li>
<li>Services running on the ports</li>
<li>Device uptime</li>
<li>Whether a firewall is protecting a host or not</li>

<br />


<h2>Languages and Utilities Used</h2>
<ul><!-- start of main list-->
<li>Terminal</li> 
<li>Network Mapper utility</li>
<ul><!-- start of nested list -->
 <li>nmap "website name or host IP" (for the purpose of this lab, we will be scanning the scanme.nmap.org site which has been developed for scanning purposes)  </li>
</ul><!--end of nested list-->
</li>
</ul><!--end of main list -->

<h2>Environments Used </h2>

- <b>Kali Linux</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h3>Step 1</h3><br/>
Boot up Kali Linux virtual machine and login to virtual machine. After logging into Kali Linux virtual machine, open a terminal command window and start the Network Mapper (Nmap) utility by typing the following command in the terminal: <br />
<br />
<b><i>nmap scanme.nmap.org</i></b><br /><br />
From the scan results, there are 4 ports open showing the SSH, HTTP, nping-echo, and Elite services running on the open ports. The scan performed though only gives basic information about the ports. The next steps in the lab will go over more advanced scanning techniques in the Nmap utility <br /><br />
<img src="Images/nmap open ports.png" height="50%" width="50%"/><br />
<h3>Step 2</h3><br/>
From the SET menu, choose the "Social Engineering Attacks" option.<br /><br />
<img src="https://github.com/AndrewLSimmons/CredentialHarvestingLab/blob/8c669824b6e22f88087ea63d9b660da6f8a0b254/Images/Social%20Engineering%20Attacks.png" height="50%" width="50%"/><br />
<h3>Step 3</h3><br/>
From the social engineering attack vector list of options. Choose the "Website Attack Vectors" option.<br /><br />
<img src="https://github.com/AndrewLSimmons/CredentialHarvestingLab/blob/8c669824b6e22f88087ea63d9b660da6f8a0b254/Images/Website%20Attack%20Vectors.png" height="50%" width="50%"/>
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

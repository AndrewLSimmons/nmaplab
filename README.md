# How to Scan a Host using the Nmap Utility in Kali Linux? 
<h2>Description</h2>
The Network Mapper (Nmap) utility is a common tool used with hackers as well as system administrators to scan a network host or device such as a server, pc, router, etc. The goal of the Nmap utility is to gather information about a targeted system or network and find vulnerabilities through the open ports/services being used. <br /><br />
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
 <li>nmap "website name or host IP" (for the purpose of this lab, we will be scanning the scanme.nmap.org site which has been developed for lab purposes and is available for the public to scan.)  </li>
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
<img src="Images/nmap open ports.png" height="85%" width="85%"/><br />
<h3>Step 2</h3><br/>
To start with an advanced scan of the Nmap utility, we may want to determine versions for the services running on each port to find out if the service is out of date and is possibly vulnerable to exploitation. <br /><br />
We will run the following command at the root (sudo command) to find out the version of the services being used:<br /><br />
<b><i>sudo nmap -v -sT -sV -O scanme.nmap.org</b></i> <br /><br />
<img src="Images/nmap advanced command.png" height="100%" width="100%"/><br />
<h3>Step 3</h3><br/>
Running the Nmap utility with the -v flag did give satisfactory information but there is another way to perform a full scan with Nmap. <br /><br />
If you want to find port states and traceroute information without establishing a full TCP connection with the firewall, the TCP SYN (stealth) Scan approach can be used with the (-sS) flag in conjunction with the(-A) flag (full scan flag).<br /><br />
<img src="Images/nmap tcp syn (stealth) scan (-sS).png" height="100%" width="100%"/>
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

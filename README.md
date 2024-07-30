<h1>Nessus Vulnerability Management Lab</h1>

<!-- ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo) -->

<h2>Description</h2>
In this lab I setup Nessus essentials to scan a vulnerable Windows 10 VM with outdated software. I used Vmware Workstation player to run the Windows 10 machine, and activated Nessus Essentials on my desktop. I was able to identify the vulnerabilities that were present in the VM and take steps to remediate them through patching and uninstalling of software.
<br/><br/>
I first ran a scan of the freshly installed version of Windows 10 22H2. Nessus found many vulnerabilities with stock software and Windows updates as the OS had not run Windows update yet.
<br/><br/>
After determining my baseline, I then ran a credentialed scan using the administrator credentials I setup initially. Nessus was able to find many more high and critical vulnerabilities after this scan.
<br/><br/>
To add to the fire I installed a very outdated version of Mozilla Firefox and ran the Nessus scan once again.
<br/><br/>
After viewing all of the vulnerabilities that Firefox introduced, I then began the process of remediation by completely uninstalling Firefox 3.6.12 and running Windows Update.
<br/><br/>

Thanks to Josh Madakor for the awesome lab project: https://www.youtube.com/watch?v=lT6Px9zJM3s
<br />


<h2>Platforms and Technology Used</h2>

- <b>Tenable Nessus Vulnerability Scanner</b>
- <b>VMware Workstation Player</b>
- <b>Windows 10</b>

<h2>Environments Used </h2>

- <b>Nessus</b>
- <b>Command Prompt</b>

<h2>Project walk-through:</h2>

<p align="center">
Download Windows 10 ISO from Microsoft: <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/e28e0618-7907-42f0-b182-25c5f6b0b862" height="80%" width="80%" alt="Windows 10 Download"/>
<br />
<br />
Download and install Tenable Nessus:  <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/9a771996-0eee-40f5-a6de-5d75aa7157d1" height="80%" width="80%" alt="Tenable Nessus Download"/>
<br />
<br />
Activate Nessus Essentials with code sent to email:  <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/dcfa2f11-7636-4729-b17b-ee1284cf83b9" height="80%" width="80%" alt="Nessus Essentials Activation"/>
<br />
<br />
Initial setup of Windows 10 VM within VMWare Workstation Player:  <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/c13efe8a-7cf2-481c-9081-1266cb4fdb9d" height="80%" width="80%" alt="Windows 10 setup"/>
<br />
<br />
Disable Windows Firewall to be able to ping the VM from local machine:  <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/df4941c7-6345-48a0-a3e4-03c6d421c957" height="80%" width="80%" alt="Disable Windows Firewall"/>
<br />
<br />
Test ping from local machine to VM:  <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/16a1f1d5-bfef-4b30-9878-1f5d8adbea08" height="80%" width="80%" alt="Test Ping"/>
<br />
<br />
Setup basic network scan within Nessus targeting the IP of the VM:  <br/>
<img src="https://github.com/ZakJaeb/Nessus-Vuln-Manage/assets/58833790/0bd12d38-070e-4fe0-83ef-2078143ae627" height="80%" width="80%" alt="Basic network scan"/>
<br />
<br />

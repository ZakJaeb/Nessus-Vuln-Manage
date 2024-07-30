# Nessus-Vuln-Manage

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
Setup new resource group for lab: <br/>
<img src="https://github.com/ZakJaeb/SOC-Honeynet-Azure/assets/58833790/e3e0702e-1635-4e62-aa86-3cf8cffbf22d" height="80%" width="80%" alt="Resource Group"/>
<br />
<br />
Deploy the Windows 10 Virtual Machine:  <br/>

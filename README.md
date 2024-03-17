# Setup-of-WDS
<h1>Windows Server 2019 with DHCP - WDS Setup</h1>
<h2>Table of Contents</h2>
<ul>
  <li>Introduction</li>
  <li>Installation of WDS role on Server</li>
  <li>Configuration of WDS</li>
  <li>Deployment of Image from WDS</li>
</ul>

<h2>Introduction</h2>
<p>
  Welcome to my WDS Configuration Repository for Windows Server 2019! This repository acts as a thorough manual and resource for the setup and configuring of Windows Deployment Server on a Windows Server 2019 machine. This manual assumes a couples things: 
  <ol>
    <li>You already have a network environment with Active Directory on a Windows Server 2019 machine</li>
    <li> Your network is setup with DHCP already</li>
    <li>You have a machine with no OS on it that will be PXE booted on the network</li>
  </ol>
  This repository offers comprehensive instructions and configurations designed to make the installation and configuration procedure as simple as possible for myself incase I need a refresher, however, it should be easy enough to understand for another administrator to follow for a refresher for themself as well. The main setup will be done on my management server with a GUI.
</p>

<h2> What is WDS and Why do you need it?</h2>
<p>WDS is an acronym for Microsoft’s Windows Deployment Services. Windows Deployment Services is used by network administrators to deploy a Windows Operating System over a network. Remember, usually if you have to deploy Windows on several systems you would have to go through a long tedious process of going to each device with a CD or a FlashDrive and install windows one by one.
<br>
<br>
WDS is particularly useful in large organizations where deploying the OS manually on each machine is time-consuming. WDS also provides a centralized management console that allows administrators to manage and configure deployment settings from a single location. This simplifies the deployment process and ensures consistency across all installations.
<br>
<br>
You can read more about WDS here: https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831764(v=ws.11)
</p>

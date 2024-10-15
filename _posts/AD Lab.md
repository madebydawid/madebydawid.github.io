---
title: Hello and welcome
date: 2024-1004-17 13:40 +0200
categories: #[homelab,hardware]
tags: #[servers,vmware]     # TAG names should always be lowercase
---
<img src="https://images.unsplash.com/photo-1683322499436-f4383dd59f5a?q=80&w=2671&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="A beautiful landscape" width="100%" height="300px" style="object-fit: cover;" />


# Active Directory and PowerShell Home Lab
**Post Author:** Dawid  
**Category:** IT / Projects  
**Last Modified:** April 17, 2024  

## Project Purpose
A few weeks ago, I decided to kick off an IT hobby project. I was inspired by [Josh Madakor](https://www.youtube.com/c/JoshMadakor), whom you can find on YouTube. The purpose was to expose myself to new technologies I haven’t worked with much, and because it's fun to tinker with computers, networks, and related stuff.

I planned to create a home lab in a virtual environment using Oracle VM VirtualBox. The idea was to set up a Windows Server 2019 as a Domain Controller with Active Directory, hosting over 1000 user accounts. These accounts would be created using a generated name list and a PowerShell script. The aim was to simulate a large company with many users.

## Software requirements
List of necessary software for the project:

- Oracle software for virtualization
- Windows Server 2019
- Windows 10

All of these ire free to download for a project like this.

## What Did I Learn?
A project of this scale, whether extensive or simple, takes time. Maybe that’s because I could only spend an hour here and there. But things take time to set up, configure, troubleshoot, and all those Windows restarts (Oh Lord!). Since I documented the entire process, it probably took much longer than it would have if I’d only focused on the installation itself. But because I wanted to document it as I went along, it took extra time.

I gained hands-on experience working with Windows Server, DHCP, DNS, RAS/NAT, and other interesting areas. Unfortunately, I didn’t encounter any major issues along the way—most of it went smoothly. I say “unfortunately” because it’s precisely when problems arise that the opportunity for growth and problem-solving appears. The most challenging part was the PowerShell scripting. I’m used to navigating Linux bash, but I have limited experience with PowerShell or scripting in general. However, this is something I definitely want to explore more.

One thing is certain: I’ll absolutely repeat the project in the future, maybe when I have a full day to spare and can skip the documentation altogether. Then I’ll focus solely on installation and configuration.

If you’d like to check out the project and give it a try yourself, you’re more than welcome to visit my [GitHub](https://github.com/madebydawid/ActiveDirectoryLab). There you’ll find step-by-step instructions on how the entire process went.


//Cheers

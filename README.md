Over the past couple weeks, I've been looking to shore up my experience and knowledge in an IT Support or helpdesk context in order to get better grasp on how I may actually operate in the position. There is only so much reading and "book-smarts" that one can build before the need for hands-on application and experience become crucial. I've seen this in my time spent studying with UMGC. In my opinion, this not only applies to mainly technical fields, but even the more intangible ones such as sociology or psychology. The practical application of learned knowledge enhances our fundamental understanding of the subject, but often provides even more valuable growth opportunities. For example, I know about Active Directory and the various Windows Administrative tools, but never really had a reason to delve deeper. Now ask me how to do specific tasks according to specific problems? There may be a bit of an issue there. That is why I found the virtual/simulated lab portions of me studies to be extremely rewarding. 

Previously I've used a professional license of VMware provided by various courses. However, I have moved to VirtualBox due to it being free, but still extremely capable. I already had a Windows 2022 Server and Windows 10 Pro VM created and ready to go. However, there were a few things I did to tune it for the purposes of learning more about a helpdesk role.

Checkout 𝗞𝗲𝘃𝗶𝗻 𝗔𝗽𝗼𝗹𝗶𝗻𝗮𝗿𝗶𝗼 of https://www.youtube.com/@KevtechITSupport for some powerful, free, approachable knowledge!


## 🧪 IT Support Lab Series

This series of labs walks through hands-on, practical IT support scenarios built in a home lab environment using VirtualBox, Windows Server 2022, Windows 10 Pro, and various industry tools. Each lab focuses on skills relevant to entry-level help desk, sysadmin, and GRC-aligned roles.

### 🔗 Lab Index

1. [**Lab Setup – Part 1**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/lab-setup-part1.md)  
   Initial setup of Windows Server and Windows 10 Pro virtual machines in VirtualBox, including configuration for domain controller and network settings.

2. [**Lab Setup – Part 2**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/lab-setup-part2.md)  
   Domain join process, Active Directory Domain Services (ADDS) setup, and testing workstation-to-server connectivity.

3. [**AD Permissions & Shared Drives**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/ad-permissions.md)  
   Created and tested security groups, delegated permissions, and configured folder sharing using NTFS and AD best practices.

4. [**Remote Desktop & Group Policy**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/remote-desktop-gpo.md)  
   Configured RDP access and applied Group Policy Objects (GPOs) for administrative control over user environments.

5. [**Silent Software Deployment with PDQ**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/pdq-deployment.md)  
   Used PDQ Deploy and Inventory to silently push applications across machines and track software installations.

6. [**Printer Access & Permissions in AD**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/printer-access-control.md)  
   Managed network printer sharing through Active Directory with customized access control based on security groups.

7. [**Spiceworks Remote Support & AD Tools**](https://github.com/DCodeDavonte/IT-Support-Lab-Series/blob/main/spiceworks-ad-tools.md)  
   Explored help desk workflow using Spiceworks Cloud, and tested AD Delegation and account lockout troubleshooting tools.
---
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th colspan="2" style="text-align: center;">Silent Software Deployment &amp; Inventory (PDQ)</th>
</tr>
</thead>
<tbody>
<tr>
<td>Task/Process</td>
<td>Knowledge Gained</td>
</tr>
<tr>
<td>Silent Software Deployment (PDQ)</td>
<td>Executed remote, unattended software installations to streamline endpoint management and minimize user disruption.</td>
</tr>
<tr>
<td>Targeting Deployments via Active Directory</td>
<td>Utilized Active Directory integration to deploy software based on domain membership and organizational unit targeting.</td>
</tr>
<tr>
<td>Creating and Deploying Custom MSI Packages</td>
<td>Built and deployed custom installation packages to overcome default deployment failures and adapt to machine-specific conditions.</td>
</tr>
<tr>
<td>Collecting System Information through PDQ Inventory</td>
<td>Queried and centralized system data including OS version, user sessions, and hardware specs for audit and reporting purposes.</td>
</tr>
<tr>
<td>Executing Remote Commands via PDQ Inventory</td>
<td>Ran diagnostics on remote endpoints using command-line tools through PDQ’s command execution feature to retrieve network configuration and status.</td>
</tr>
<tr>
<td>Troubleshooting Deployment Failures on a Server</td>
<td>Diagnosed and resolved installation issues by identifying network adapter conflicts and manually configuring alternative deployment methods.</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th colspan="2" style="text-align: center;">Remote Desktop Services &amp; Group Policy Management</th>
</tr>
</thead>
<tbody>
<tr>
<td>Task/Process</td>
<td>Knowledge Gained</td>
</tr>
<tr>
<td>Enabling Remote Desktop (RDP)</td>
<td>Configured remote desktop settings and troubleshot connectivity issues to establish seamless remote access between systems.</td>
</tr>
<tr>
<td>Testing Connectivity Between Machines</td>
<td>Diagnosed and resolved network connectivity issues using command-line tools to ensure proper communication between systems.</td>
</tr>
<tr>
<td>Accessing Shared Drives</td>
<td>Managed shared drive access through File Explorer and Registry Editor, ensuring efficient and secure file management.</td>
</tr>
<tr>
<td>Connecting to Remote Registry</td>
<td>Administered remote registry access to configure system settings and troubleshoot remote machine issues, enhancing IT management.</td>
</tr>
<tr>
<td>Using Group Policy for Restrictions</td>
<td>Deployed and enforced Group Policy settings to restrict shutdown/restart access, preventing accidental system downtime.</td>
</tr>
<tr>
<td>Firewall Configuration for Remote Access</td>
<td>Configured firewall rules to allow ICMP and SMB traffic, ensuring uninterrupted remote access while maintaining network security.</td>
</tr>
<tr>
<td>Remote Troubleshooting and User Support</td>
<td>Utilized remote desktop and registry tools to troubleshoot system issues and provide support without physical access to the machine.</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th colspan="2" style="text-align: center;">Active Directory &amp; Shared Drive Permissions</th>
</tr>
</thead>
<tbody>
<tr>
<td>Task/Process</td>
<td>Knowledge Gained</td>
</tr>
<tr>
<td>Useful Commands</td>
<td>Gained practical knowledge in useful commands like <strong>ping</strong>, <strong>gpresult</strong>, and <strong>gpupdate</strong> for network troubleshooting and Group Policy management.</td>
</tr>
<tr>
<td>Account Lockout &amp; Disabled Accounts</td>
<td>Learned to manage locked, disabled, and expired accounts in Active Directory, ensuring users regain access.</td>
</tr>
<tr>
<td>Rejoining Computer to Domain</td>
<td>Gained hands-on experience troubleshooting and rejoining computers that have fallen off the domain.</td>
</tr>
<tr>
<td>Creating Shared Drives &amp; Configuring Permissions</td>
<td>Developed skills in creating shared drives, setting up security groups, and applying granular access controls to shared resources.</td>
</tr>
<tr>
<td>Mapping Network Drives</td>
<td>Acquired experience in mapping network drives for user-specific access to shared folders, ensuring proper access controls.</td>
</tr>
<tr>
<td>Configuring Personal Folder Mapping</td>
<td>Learned to configure individualized network drives for users, linking to their dedicated folders for personalized access.</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th colspan="2" style="text-align: center;">Lab Setup Part 2</th>
</tr>
</thead>
<tbody>
<tr>
<td>Task/Process</td>
<td>Knowledge Gained</td>
</tr>
<tr>
<td>Creating a Second Virtual Machine</td>
<td>Gained experience in creating and configuring a second VM (Desktop2) to simulate a user workstation in a network.</td>
</tr>
<tr>
<td>Configuring Organizational Units (OUs)</td>
<td>Learned to create and organize OUs within Active Directory and move users into appropriate units based on roles.</td>
</tr>
<tr>
<td>Using the Attribute Editor</td>
<td>Acquired skills in using the Attribute Editor to manage and view detailed information about AD objects (e.g., users, OUs).</td>
</tr>
<tr>
<td>Managing Group Policies</td>
<td>Gained knowledge in accessing and editing group policies and enforcing domain-wide security settings and restrictions.</td>
</tr>
<tr>
<td>Adding Machines to Network/Domain</td>
<td>Learned how to configure a static IP, ensure network connectivity, and join a machine to the domain for integration into a network environment.</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 49%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th colspan="2" style="text-align: center;">Lab Setup Part 1</th>
</tr>
</thead>
<tbody>
<tr>
<td>Task/Process</td>
<td>Knowledge Gained</td>
</tr>
<tr>
<td>Virtual Machine Networking</td>
<td>Practical experience with virtualized environments, managing virtual networks, and IP settings.</td>
</tr>
<tr>
<td>Firewall Management</td>
<td>Skills in configuring firewall rules and managing security without compromising connectivity.</td>
</tr>
<tr>
<td>RSAT Tools Installation</td>
<td>Experience installing and using remote server management tools on client machines for domain management.</td>
</tr>
<tr>
<td>Networking Configuration</td>
<td>Knowledge of IP configuration, static IPs, and troubleshooting connectivity issues between devices.</td>
</tr>
<tr>
<td>Active Directory Setup</td>
<td>Understanding of AD Domain Services, creating domains, user/group management, and permissions.</td>
</tr>
</tbody>
</table>


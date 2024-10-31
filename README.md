<h2>🖥️ Active Directory Home Lab</h2>

<h3>Project Overview</h3>
<p>This project demonstrates the setup of a <strong>Windows Active Directory (AD) environment</strong> in a home lab, designed for <strong>cybersecurity and IT administration practice</strong>. Active Directory is a crucial component in enterprise environments, used for managing users, groups, permissions, and policies across a network. Setting up an AD lab allows for hands-on learning and testing in a controlled environment, making it an essential tool for cybersecurity professionals to understand network administration, user management, and security protocols.</p>

<h3>Goals of This Lab</h3>
<ul>
    <li>Gain practical experience in <strong>Active Directory administration</strong> and <strong>Windows Server management</strong>.</li>
    <li>Explore <strong>Group Policy Objects (GPO)</strong>, user authentication, permissions, and access control.</li>
    <li>Simulate <strong>cybersecurity attacks and defenses</strong> within an AD environment, including techniques like privilege escalation and lateral movement.</li>
    <li>Develop and test <strong>PowerShell scripts</strong> for user and system management.</li>
</ul>

<h3>Lab Setup Details</h3>
<p>The lab setup includes:</p>
<ul>
    <li><strong>Windows Server 2019/2022</strong>: Configured as the Domain Controller (DC) for managing the Active Directory environment.</li>
    <li><strong>Linux Clients</strong>: Joined to the domain to simulate an enterprise network with Linux devices.</li>
    <li><strong>Virtual Network</strong>: A secure, isolated virtual network where the domain controller and clients can communicate.</li>
</ul>

<h3>Key Components</h3>
<ul>
    <li><strong>Domain Controller (DC)</strong>: This is the heart of the Active Directory, responsible for user authentication and enforcing security policies.</li>
    <li><strong>Active Directory Users and Computers (ADUC)</strong>: Used to manage users, groups, and computers within the domain.</li>
    <li><strong>Group Policy Management</strong>: Configured to enforce security policies across the network, such as password policies, account lockout settings, and software installation restrictions.</li>
    <li><strong>DNS Server</strong>: Installed on the Domain Controller to handle name resolution within the domain.</li>
    <li><strong>PowerShell Scripts</strong>: Automated scripts used to streamline administrative tasks and improve efficiency.</li>
</ul>

<h3>Step-by-Step Setup Process</h3>
<ol>
    <li><strong>Install Windows Server</strong>: Set up a Windows Server VM (Virtual Machine) to act as your Domain Controller.</li>
    <li><strong>Promote Server to Domain Controller</strong>: Configure the server as a Domain Controller and set up your domain (e.g., <code>lab.local</code>).</li>
    <li><strong>Install AD DS and DNS Roles</strong>: Add the Active Directory Domain Services (AD DS) and DNS roles to enable directory services and network name resolution.</li>
    <li><strong>Create Organizational Units (OUs)</strong>: Organize users, groups, and computers into OUs for easier management.</li>
    <li><strong>Configure Group Policy Objects (GPOs)</strong>: Set up policies for user account security, software restrictions, and other controls.</li>
    <li><strong>Add Client Machines</strong>: Set up Linux VMs, join them to the domain using tools like <code>sssd</code> and <code>realmd</code>, and verify connectivity with the Domain Controller.</li>
    <li><strong>User and Group Management</strong>: Create test user accounts, groups, and assign them to specific OUs for testing GPOs and permission settings.</li>
    <li><strong>Simulate Security Scenarios</strong>: Test security policies, such as user account lockouts, restricted access, and privileged account management.</li>
</ol>

<h3>Security and Attack Simulations</h3>
<p>To build defensive skills, the lab includes simulations of common attack vectors within an AD environment:</p>
<ul>
    <li><strong>Privilege Escalation</strong>: Attempt escalation of permissions within the lab to understand how attackers may gain unauthorized access.</li>
    <li><strong>Lateral Movement</strong>: Simulate lateral movement across devices in the domain to understand potential attack paths and how to secure them.</li>
    <li><strong>Password Policies</strong>: Test different password policies and monitor for security issues related to weak passwords.</li>
</ul>
  
<h3>Tools Used</h3>
<ul>
    <li><strong>Virtualization Software</strong>: VMware Workstation or VirtualBox for setting up virtual machines.</li>
    <li><strong>Windows Server 2019/2022</strong>: Domain Controller.</li>
    <li><strong>Linux (e.g., Ubuntu, CentOS)</strong>: Client machines.</li>
    <li><strong>PowerShell</strong>: For scripting and automation on Windows Server.</li>
    <li><strong>Wireshark</strong>: Network analysis and traffic inspection.</li>
    <li><strong>Nmap</strong>: Network discovery and port scanning for lab testing.</li>
</ul>

<h3>Why This Lab is Important</h3>
<p>This Active Directory lab provides an isolated environment to practice <strong>network security</strong> and <strong>AD management</strong> skills without risking production systems. By testing policies, permissions, and security controls in this lab, you gain valuable experience with real-world scenarios. It also allows for experimentation with penetration testing techniques in a controlled setup, making it a powerful learning tool for cybersecurity professionals.</p>

1. What is Operating System Security?

Operating System (OS) Security refers to protecting the OS from:

Unauthorized access

Malware

Misuse of system resources

Data leakage

📌 The OS is the first line of defense in any system.

2. User Authentication & Authorization
Linux:

Authentication via /etc/passwd and /etc/shadow

Uses username + password

Supports SSH keys

Permission-based access

Windows:

Authentication via Active Directory / SAM

Uses username + password / PIN / biometrics

Supports Kerberos authentication

Exam Point:
Authentication = Who you are
Authorization = What you can access

3. File System Permissions
Linux File Permissions:

Read (r) – view file

Write (w) – modify file

Execute (x) – run file

Permission format:

-rwxr-xr--


Owner | Group | Others

Windows File Permissions:

Uses NTFS permissions

Read, Write, Modify, Full Control

Managed through ACLs (Access Control Lists)

📌 Incorrect permissions lead to privilege escalation.

4. User Privilege Management
Linux:

Root user (superuser)

sudo command for temporary privilege escalation

Principle of Least Privilege

Windows:

Administrator account

User Account Control (UAC)

Role-based access

Exam Line:
Least privilege reduces damage if an account is compromised.

5. Patch Management & Updates
Linux:

Package managers: apt, yum, dnf

Regular kernel and software updates

Windows:

Windows Update

Patch Tuesday releases

Automatic security updates

📌 Unpatched systems are easy targets for attackers.

6. Malware Protection
Linux:

Less targeted but still vulnerable

Tools: ClamAV, SELinux, AppArmor

Windows:

Highly targeted by malware

Windows Defender, Antivirus software

Real-time protection

Exam Point:
Windows needs stronger malware protection due to high usage.

7. Firewall & Network Security
Linux Firewall:

iptables

ufw

firewalld

Windows Firewall:

Windows Defender Firewall

Inbound and outbound rules

📌 Firewalls control network traffic and block unauthorized access.

8. Logging & Monitoring
Linux Logs:

/var/log/auth.log

/var/log/syslog

/var/log/messages

Windows Logs:

Event Viewer

Security logs

Application & System logs

SOC Relevance:
Logs help detect attacks and investigate incidents.

9. Disk & Data Protection
Linux:

Disk encryption using LUKS

Secure file permissions

Windows:

BitLocker encryption

Encrypted File System (EFS)

📌 Encryption protects data if a system is stolen.

10. Secure Boot & System Hardening
Linux:

OS Security Checklist 
1. User & Access Control

Use strong passwords

Enable MFA where possible

Apply Principle of Least Privilege

Disable unused accounts

2. Authentication & Login Security

Lock account after failed attempts

Disable root/Administrator direct login (where applicable)

Secure remote access (SSH/RDP)

3. Patch & Update Management

Enable automatic OS updates

Regularly update applications and drivers

Remove unsupported software

4. File System & Permissions

Set correct file/folder permissions

Protect sensitive system files

Use NTFS ACLs (Windows) / rwx permissions

Disable unused services

Secure SSH

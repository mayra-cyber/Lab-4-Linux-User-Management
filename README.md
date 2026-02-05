# Lab 4 — Linux User, Group & Permission Management

## Objective
Practice Linux user and group management by creating, modifying, and removing accounts, assigning permissions, and controlling sudo access to simulate security and breach scenarios.

## Environment
- Host OS: Windows  
- Hypervisor: VirtualBox  
- Guest OS: Linux  
- Network Mode: NAT  

## Tools Used
- Linux Terminal
- sudo
- visudo
- useradd / adduser
- usermod
- groupadd
- gpasswd
- userdel
- /etc/passwd
- /etc/group

## What I Built
- Created multiple user accounts
- Assigned and modified passwords
- Created and deleted groups
- Granted and revoked sudo privileges
- Simulated a breach using an unauthorized user
- Removed compromised users
- Restored system control using group-based permissions

## Breach Simulation
- Created a malicious user (black_widow)
- Gained unauthorized sudo privileges
- Added and deleted users
- Used a privileged group (magic) to restore control
- Removed attacker from sudo access
- Deleted unauthorized accounts
- Cleaned up privileged groups

## Outcome
Successfully created, modified, and secured multiple user accounts and groups. I was able to detect, control, and remove an unauthorized user using Linux privilege management.

## Reflection
This lab showed how dangerous sudo access can be if misconfigured and how Linux groups and permissions can be used to regain control after a breach. I also learned the difference between adduser and useradd, including how home directories are created.

---

## Screenshots

### User Creation & Configuration
![User creation](Screenshots/01_user_creation.png)
![Password setup](Screenshots/02_user_password_set.png)
![User shell update](Screenshots/03_user_shell_and_passwd.png)

### System Audit
![User audit](Screenshots/04_passwd_user_audit.png)
![Audit after changes](Screenshots/05_passwd_after_changes.png)

### Privilege Management
![User switching](Screenshots/06_user_switch_and_privileges.png)
![Visudo configuration](Screenshots/07_visudo_privilege_management.png)
![Sudoers privilege assignment](Screenshots/09_sudoers_privilege_assignment.png)

### Filesystem & Group Management
![Home directory permissions](Screenshots/10_home_directory_permissions.png)
![Group membership verification](Screenshots/11_group_membership_verification.png)
![Remove user from group](Screenshots/12_remove_user_from_group.png)

### Incident Cleanup & Final Verification
![System cleanup](Screenshots/13_system_cleanup_final.png)
![Final system audit](Screenshots/14_final_system_audit.png)

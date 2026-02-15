# Windows Basics for Cybersecurity

These notes cover Windows fundamentals
important for cybersecurity and system understanding.
The focus is on how Windows works under the hood,
not on exploitation.

---

## 1. What Is Windows

Windows is a widely used operating system for:
- personal computers
- corporate environments
- enterprise networks

Many corporate infrastructures rely heavily on Windows,
especially with Active Directory.

---

## 2. Windows Architecture (High-Level)

Windows consists of:
- kernel (core of the system)
- user mode processes
- system services

Key idea:
Applications do not talk directly to hardware.
The kernel controls access.

---

## 3. Users and Accounts

Windows uses user accounts to control access.

Common account types:
- local user
- local administrator
- domain user

Each user has:
- a username
- a SID (Security Identifier)
- assigned permissions

---

## 4. User vs Administrator

### Standard User
- limited permissions
- cannot modify system-wide settings
- safer for daily use

### Administrator
- full system access
- can install software
- can modify system configuration

Running as administrator increases risk.

---

## 5. User Account Control (UAC)

UAC is a security feature in Windows.

Purpose:
- prevent silent privilege escalation
- require confirmation for admin actions

Even administrators run with limited rights
until elevation is approved.

---

## 6. Windows File System (NTFS)

Windows primarily uses the NTFS filesystem.

Key features:
- file permissions
- file ownership
- auditing
- encryption support

Paths use backslashes:
```text
C:\Users\Username

---

## 7. NTFS Permissions (Basic)
NTFS permissions control access to files and folders.

Common permissions:
- Read
- Write
- Modify
- Full Control

Permissions can be assigned to:
- users
- groups
Permissions are cumulative unless explicitly denied.

---

## 8. Windows Processes
A process is a running program.

Each process has:
- a PID (Process ID)
- a user context
- assigned permissions

---

## 9. Viewing Processes
Task Manager
- GUI-based process viewer:
- shows CPU, memory, disk usage

Shortcut:
Ctrl + Shift + Esc

Command Line
tasklist

---

## 10. Windows Services

Services are background processes
that start automatically or manually.

Examples:
- Windows Update
- Event Log
- Antivirus services

Services often run with high privileges.

---

## 11. Windows Command Line Interfaces

Windows provides multiple command-line tools:
- Command Prompt (cmd)
- PowerShell
PowerShell is more powerful and scriptable.

---

## 12. Basic Command Prompt Commands
- whoami
- dir
- cd
- ipconfig

Command meanings:
- whoami – show current user
- dir – list files
- cd – change directory
- ipconfig – show network configuration

---

## 13. Event Logs (High-Level)

Windows records system activity in event logs.

Types of logs:
- Application
- Security
- System

Logs are critical for:
- troubleshooting
- incident investigation
-- security monitoring

---

Key Takeaways:
- Windows dominates enterprise environments
- users and permissions control access
- administrators are high-risk targets
- NTFS enforces file security
- processes and services define system behavior
- logs are essential for visibility

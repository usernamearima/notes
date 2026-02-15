# Linux Basics for Cybersecurity

These notes cover Linux fundamentals commonly used
in cybersecurity, networking, and system administration.
All content is for learning and legal use only.

---

## 1. What Is Linux

Linux is an operating system commonly used for:
- servers
- security tools
- development
- cloud environments

Linux is controlled mainly through the terminal,
not through a graphical interface.

---

## 2. Terminal Basics

The terminal allows controlling the system using commands.

You use it to:
- move between directories
- inspect files
- manage the system

### Basic Commands
```bash
pwd
ls
cd
```
## Command Meanings

- `pwd` – show current directory  
- `ls` – list files and folders  
- `cd` – change directory  

---

## 3. File and Directory Navigation

### Examples
```bash
cd /home
cd ..
cd ~
ls -la
```
Important concepts:
/ is the root directory
.. means parent directory
~ means user home directory

---

## 4. Nano Text Editor

Nano is a simple terminal-based text editor.

### Open a File
```bash
nano filename
```
You type text normally.

Controls:
Ctrl + O – save file
Enter – confirm filename
Ctrl + X – exit editor

Nano Is Commonly Used For:
- configuration files
- scripts
- notes

---

## 5. Linux File Permissions

Linux controls who can read, write, and execute files.

### Permission Types
- `r` – read  
- `w` – write  
- `x` – execute  

### Permission Groups
- `u` – owner  
- `g` – group  
- `o` – others  

---

## 6. chmod – Changing Permissions

`chmod` changes file permissions.

### Example
```bash
chmod +x script.sh
```
This allows the file to be executed.

Permissions Are Critical For:
- security
- preventing unauthorized access
- controlling script execution

---

## 7. chown – Changing Owner

chown changes the owner of a file.

Example:
- chown kali file.txt
Ownership controls who can modify or manage files.

---

## 8. Users, Root, and Privileges

Linux has different privilege levels:
- normal user → limited permissions
- root (administrator) → full control

---

## 9. sudo

sudo allows running a single command as administrator.

Important Points:
- uses the user's password
- privileges are temporary
- reduces risk compared to full root login

Example:
sudo apt update

---

## 10. Becoming Root
Method 1 (common)
sudo su

Method 2 (recommended)
sudo -i

When logged in as root:
- prompt usually ends with #

Exit root:
- exit

---

## 11. Package Management with apt

Linux installs software from repositories.

apt:
- downloads software
- installs it
- manages dependencies

---

## 12. Updating the System
sudo apt update
sudo apt upgrade

Often combined:
sudo apt update && sudo apt upgrade

Keeping the system updated is critical for security.

---

## 13. Installing Software

Install Programs:
- sudo apt install curl
- sudo apt install git
- sudo apt install htop

Check if Installed
program --help
which program

Remove Software
sudo apt remove program

---

## 14. Linux Filesystem Structure

Linux has one main directory: /

Important Directories:
/ – root
/home – user files
/etc – configuration files
/bin, /usr – system programs
/var – logs
/tmp – temporary files

Understanding the filesystem is key to system navigation.

---

## 15. Processes

A process is a running program.

View Processes
ps

Live View
top

Enhanced View (if installed)
htop

---

## 16. Managing Processes

You can:
- see what is running
- check CPU and RAM usage
- stop unresponsive programs

Kill a Process
kill PID

PID = Process ID.

Key Takeaways
- Linux is terminal-focused
- permissions control access
- sudo limits risk
- apt manages software
- filesystem structure matters
- processes must be monitored

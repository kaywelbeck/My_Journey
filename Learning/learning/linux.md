<div style="text-align: center;">
    <h1><u>LINUX</u></h1>
</div>

<h4><u>WHAT IS LINUX</h4></u>

<span style="color:green;">OS</span> handles interactions between apps and hardware

LINUX is an <span style="color:green;">open source</span> operating system
<span style="color:purple">open source:</span> is source code that can be inspected,modified and enhanced by anyone.

- supports multiple users and multi-tasking
- is built to handle networking
- Provides system tools and utilities
---
<h4><u>Major Components of a Linux Distribution</u></h4>

1. **<span style="color:green">Kernel</span>**
   - **Role**: The <span style="color:green">kernel</span> is the core component of the Linux operating system. It acts as a bridge between the hardware and software, managing system resources and allowing different applications to communicate with the hardware. 
   - **Responsibilities**:
     - **<span style="color:green">Process Management</span>**: Manages the creation, scheduling, and termination of processes.
     - **<span style="color:green">Memory Management</span>**: Handles the allocation and deallocation of memory resources.
     - **<span style="color:green">Device Management</span>**: Manages communication between the system and hardware devices (e.g., keyboards, monitors, storage).
     - **<span style="color:green">File System Management</span>**: Organizes and manages data on storage devices.

2. **<span style="color:green">Daemons</span>**
   - **Role**: <span style="color:green">Daemons</span> are background services that provide extra support for the system or user. These processes typically run in the background and perform various tasks without user interaction.
   - **Examples**:
     - **<span style="color:green">System Services</span>**: Services like `cron` (for scheduled tasks) and `sshd` (for remote access via SSH).
     - **<span style="color:green">Network Services</span>**: Services such as web servers (e.g., Apache) and database servers (e.g., MySQL).

3. **<span style="color:green">Applications</span>**
   - **Role**: <span style="color:green">Applications</span> are user-level programs that allow users to perform specific tasks. These include a wide variety of software that runs on top of the Linux system.
   - **Examples**:
     - **<span style="color:green">Productivity</span>**: Text editors (e.g., Vim, Nano), word processors (e.g., LibreOffice Writer).
     - **<span style="color:green">Multimedia</span>**: Music players, video players.
     - **<span style="color:green">Internet Browsing</span>**: Web browsers like Firefox and Chrome.

4. **<span style="color:green">Data Files</span>**
   - **Role**: <span style="color:green">Data files</span> consist of user-generated content or files created by applications. These files can be stored in various formats and are typically created, modified, and accessed by users or applications.
   - **Examples**:
     - **<span style="color:green">Documents</span>**: Text files, spreadsheets.
     - **<span style="color:green">Media</span>**: Images, audio files, video files.
     - **<span style="color:green">Database Files</span>**: Structured data stored in databases.

5. **<span style="color:green">Configuration Files</span>**
   - **Role**: <span style="color:green">Configuration files</span> contain settings and preferences for the Linux system, services, and applications. These files are usually stored in text format and allow administrators or users to customize the behavior of the system and applications.
   - **Examples**:
     - **<span style="color:green">System Configuration</span>**: Files in `/etc/` that control system behavior (e.g., network configuration, user permissions).
     - **<span style="color:green">Service Configuration</span>**: Configuration files for daemons, such as Apache or Nginx.
     - **<span style="color:green">Application Configuration</span>**: User-specific settings, often stored in hidden files (e.g., `.bashrc` for shell settings).
---
<img src="https://media.licdn.com/dms/image/v2/C4E12AQFPJMxJ87FUrA/article-cover_image-shrink_423_752/article-cover_image-shrink_423_752/0/1639128678129?e=1730332800&v=beta&t=o1xlDB2F1orEm7qlhF-Tt_EonOIHpOKPhfgk2DDPuO4">
<h4><u>How to interface: CLI</h5></u>

- It consumes fewer hardware resources.
- It can be automated with scripts.
- It provides more options.
- Most Linux servers use only the CLI.

<h4><u>How to interface: GUI</u></h4>

- It is visual and intuitive to navigate.
- It is similar in Linux, Microsoft Windows, and macOS.
- Most user workstations use the GUI

<img src="https://cdn.ttgtmedia.com/rms/onlineimages/advantages_of_cli_and_gui-f.png">

---

  # linux notes

  - aws@surfacelaptop5
  - aws is my username (name i use to log into the system)
  - surfacelaptop5 is my hostname (name of the computer)
  - sudo (gives tempoary admin privelages to do task)
  - advanced package tools (pach - package manager to install ubuntu, debian etc linux)
  - ncal (calender utility)
  - touch filename.txt (create a new file - filename.txt file)

  1. For the history command, it is stored in /home/username/ .bash_history
  
  ---
<h4><u>USERS AND GROUPS</u></h4>

- **<span style="color:green;">Admin Group - </span>** (super user/supervisor) `root #`
- **<span style="color:green;">Users group - </span>** (regular access) `user` (Windows `$`) (Mac `%`)

#### **User Management Commands**

- **Create User**:
  ```bash
  Useradd <username>
  ```
- **check users created**
  ```bash
  tail /etc/passwd
  ```
- **Modify User (Add Comment):**
  ```bash
  sudo usermod -c 'Julie is an AWS engineer' Julie
  ```
- **Modify User (Add Expiry Date):**
  ```bash
  sudo usermod -e 2024-08-28 Julie
  ```
- **Delete User:**
  ```bash
  sudo userdel Julie
  ```
- **Add Password**
  ```bash
  passwd Julie
  ```
- **Log in using the new users**
 ```bash
 su
 ```
- **switch to the previous user**
 ```bash
 exit
 ```
---
## **GROUPS**

**_Groups_** are useful for managing multiple user permissions.

### **Commands for Group Management**
 
- **Create a New Group**:
  ```bash
  groupadd <group_name>
  ```
- **Modify an Existing Group:** 
  ```bash
  groupmod -n <new_group> <old_group>
  ```
- **Delete Group**:
  ```bash
  groupdel <group_name>
  ```
- **To add user to group**
 ```bash
  sudo usermod -a -G <group name> <user ID>
  ```
---
## **File Editors**

### vim(works in command line)
i insert
:q quit
:wq write and save (save and wuite)

### nano (works in command line)

menu is at the bottom

nano newfile.txt

# WORKING WITH LINUX FILE SYSTEM
ls lists directory and files
ls -L lists directory and files in long format with details
 
### hash
shows history of recently used commands
# cksum filename.txt
shows cksum no. and file size of files to verify integrity
#### find /home/student -name filename.txt
helps find files
#### grep
find text or string in a file or document
#### diff
used to compare two files
 
#### absolute and relative paths
- absolute path (full file path) /mnt/c/Users/studentname/Downloads/Netcom/GBLON7
 
- relative path (abbreviated file path)
~/Downloads/Netcom/GBLON7

---
dsdfdsf

---
<h4><u>Working with Commands</u></h4>

---

daemons - special processes that are started when the system is started and stopped when the system is shut down

process - is an active program that is exuctuted 

questions?
why do we have granular permission files?


<h4><u>Managing linux processes</u></h4> 

ps shows running processes and process ides
pstree shows process and sub processess
top shows real time summary of system performance 

---
<img src="https://miro.medium.com/v2/resize:fit:1400/format:webp/1*6eqkV8wi2BHdx1nW1FbzFg.jpeg">


---

<h4><u>BASH SHELL</u></h4>



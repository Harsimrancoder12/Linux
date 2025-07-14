## 25/6/2025

 # First day of training 

In first day of training, i learned about linux in detail and different types of companies. 
   
Linux is the core of the operating system, responsible for managing hardware resources and providing a platform for other software.

Linux is open source and much better than windows.Linux is known for its stability and security. 
To install Linux on laptops , there are some steps to followed: 
       
       Download Virtualbox 7.1.10
       Download Microsoft c++ visual studio 
       Download ubnut desktop 24.04.2 LTS 

The main difference between Linux and windows is  Linux is free and open source , windows are  not open source. 
Linux considered more secure due to its open-source nature, windows are less secure.
Linux is free of cost , windows are not free of cost.

Then, we discussed about different types of companies.
           
            product based companies 
            service based companies 
            startup companies

After that I learned about Booting and its types 
  
Booting - Booting is the process of starting or resetting a computer.
 It has two main types: 

   cold booting and warm booting. 

Cold booting is starting a computer from a completely powered-off state, while warm booting is restarting a computer that is already on. 

 ## 26/06/2025

  Introduction to Kernel , Shell its types and    different commands
 
Kernel -   In an operating system, the kernel is the core component that acts as a bridge between the hardware and the software.

Shell
 In an operating system, a shell acts as an interface between the user and the kernel, allowing users to interact with the system by executing commands. 

 Types of shell 
      
        Bash - Most common shell
        sh - original shell
        zsh- more features 
        fish- modern, interactive 

 Shell categories 
        1. command line shell
        3. Graphical shell

File System Structure
   
       directory              function 
       / (Root):       The top-level directory, from which all other directories branch out.
     
      /bin:            Contains executable programs .
     
      /boot:            Stores files needed for booting the system, including the kernel.
     
       /dev:            Contains device files that represent hardware devices.
     
       /home:           Personal directories for users. 
     
       /lib:             Contains library files that are used by programs.
   
       /media:            Mount point for removable media like USB drives.
    
       /mnt:             Temporary mount point for file systems.
    
       /opt:            Contains optional apps.
   
       /srv:            Contains data for services provided by the system.
     
       /tmp:            Stores temporary files.
    
      /usr:            Contains user-related programs, libraries, and documentation.
    
      /var:           Stores variable data, such as log files, user tracking data, and caches.  

  commands
  
               Commands           Description                         Syntax
   
               ls               List the contents                     ls(options)

             date          Show the current date and time .           date

             whoami         Display the current username.              whomami    

             cd               change the directory .                  cd[directory]

             mkdir              To create new directory                mkdir directory_name

             cat                Create a list with contents            cat>filename

             touch               create file without content          touch filename

             cp                  copy the files                        cp[source]

             pwd                 print the current working directory       pwd

             whereis              show location of binary ,source         whereis[command]

             whatis               To get brief information about command       whatis[command]
 
 ![VirtualBox_ubuntu_27_06_2025_08_55_27 screenshort](https://github.com/user-attachments/assets/8b6b7586-415c-44a5-b484-eef83136b3c0)


Dual Booting 
Dual-booting refers to the process of installing and running two different operating systems on a single computer, allowing the user to choose which one to use when starting the machine. 

  BARE METAL INSTALLATION 

  Bare metal installation of linux means installing the operating on a computer's hardware , without any intermediary virtualization software.


VM ware 

vm  ware is a commercial product known for its enterprise - grade  features , performence and comprehensive support .

Partitioning Schemes :
Dividing a hard disk into seperate sections .
Each section acts as an independent disk.
Help organize data and install multiple OS.

 Its Types:

 MBR(MASTER  BOOT RECORD )

 maximum 4 primary partitions . Support upto 2 TB.It stores partition info in one place.It has less flexibility.

 GPT(GUID PARTITION TABLE)

 It supports upto 128 partitions .It supports disks larger than 2 TB.More flexibile.


## 27/06/2025 
## Permissions & Shell programming:
### File and directory permissions:
`chmod` (Change mode): It is used to change the access permissions of files and directories.

Some different chmod permission notations are:<br>
 `chmod +x test.sh`:  Gives permission to run the script.<br>
 `chmod 444 test.sh`: Changes file to read-only
 
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/read-only.jpg)

*Result* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/read-only_result.jpg)


 `chmod 644 test.sh`: Changes file such that only owner can edit it. For others it remain read-only.

![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/user_writable.jpg)

*Result* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/user_writable_result.jpg)

### Redirection:
 It allows user to redirect input and output functionalities to the files or folders. 

**Types of Redirection:**
1. Overwrite Redirection (For stdout):<br>
Redirects the standard output of a command to a file. If the file exists already contain script, it will be overwritten.<br>
">" standard output<br>


2. Append Redirection (For stdout): 
Append the output to the file without compromising the existing data of the file.

![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/redirection.jpg)

![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/redirection._result.jpg)

3. Overwrite Redirection (For stdin):<br> 
Redirects the standard input of a command to a file.<br>
"<" standard input

*sorting with help of Redirection:* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/sortbyredirection.jpg)

### Pipe '|':
The pipe is used to combine two or more commands, and in this, the output of one command acts as input to another command.

*Pipe can be used for filteration.* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/pipe.jpg)

Multiple pipes can be used such as:

*to find number of file/directory with 't'* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/multi_pipe.jpg)

### File compression:
File compression reduces file size to save space or speed up transfer.
- `gzip`:
  -  Used to zip a file.
  -  Limitation: The original file is deleted.
- `gunzip`:
  - Unzips the file.
- Flag `-k`:
  - To zip the file
  - Original file isn't deleted.

![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/gzip.jpg)

## Assignment:

### Shell programming:
1. Use of variables:
   
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/shell_variable_GNU.jpg)

*Output* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/shell_variable.jpg)

2. Multiplication table of any number:

![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/shell_table_GNU.jpg)

*Output* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/shell_table.jpg)

3. Comparing two variables:
   
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/shell_compare_GNU.jpg)

*Output* <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/shell_compare.jpg)

### `chown`:
`chown` (short for change owner) is a command used to change the ownership of a file or directory.

**How to Use `chown`:**
 1. Check current ownership (optional).
 2. Run the `chown` command.  Use `sudo` if you're not the current owner.

**Changing owner only:**<br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/chown.jpg)

**Changing group only:**<br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/chown_group.jpg)

**Changing both group and owner permissions:** <br>
![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/chown_group-own.jpg)

### Wild cards:

| Wildcard | Meaning                                       | 
| -------- | --------------------------------------------- |
| `*`      | Matches **zero or more** characters           | 
| `?`      | Matches **exactly one** character             |
| `[abc]`  | Matches **one character** from set            | 


![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/wildcard.jpg)



## Other short topics:
### Partitioning Scheme:

A **partitioning scheme** is the way a hard disk or SSD is **divided into sections** (partitions) so the system can use it properly.

**Its is used for:**<br>
* Separate **system files** from **user files**
* Install **multiple OSes**
* Create **swap space**
* Improve **backup & security**


### Types of Partitioning Schemes:

#### 1. MBR (Master Boot Record):
- Max 4 primary partitions.
- Supports up to 2 TB.
- Older, used with BIOS.
- less flexible

#### 2. **GPT (Guided Partition Table)**
- Supports 128+ partitions.
- Works with disks >2 TB.
- Newer, used with UEFI.
- more flexible

### Bare Metal Installation

* Installation directly using USB.
* Direct installation in computer hardware.
* No OS should be in between.

## 30/06/2025

Hardware 

Computer hardware refers to the physical components of a computer that you can see and touch. These components work together to process input and deliver output based on user instructions. In this article, we’ll explore the different types of computer hardware, their functions, and how they interact to make your computer work.

The computer has mainly has two major components:

Hardware
Software

          Hardware Type                         Description                                                     Example
       
       Input Devices             devices allow users to interact with
                                 a computer by entering data or commands.                                      Keyboard, Mouse, Scanner, Trackball                 
                                 These devices convert the input into a
                                 format that the computer can process.  

     
       
       Output Devices            Output devices display the results of tasks given                              Monitor,Printer,Speaker                                  
                                 to the computer in a human-readable form. 
                                                                                                                     

       Storage Devices          Some devices are used for storage purposes                                      CD (Compact disc), Hard Drive(HDD),USB
                                and are known as secondary storage devices.            
           

      Processing Unit           Components that process data and execute instructions                         CPU(Central Processing Unit),GPU(Graphics Processing Unit)

      Memory                    Temporary storage used by the CPU to hold data and instructions               RAM(Random access memory), Cache

     Motherboard               It is the main circuit board inside a computer and                              Motherboard
                               it contains most of the electronic components together.
                               All the components of the computer are directly or
                               indirectly connected to the motherboard


    Power Supply                All of a computer system's parts are powered by a power source.                  PSU(Power Supply Unit)

    Networking Hardware        Devices that connect computers and enable communication                          Network Interface Card(NIC) Router, Switch

MOTHERBOARD

Imagine your computer as a big city, and the motherboard as the main road system connecting all the important buildings—like the CPU (the brain), RAM (the memory), and storage (the library). Without the motherboard, these parts couldn’t talk to each other, and your computer wouldn’t work.A motherboard is the main circuit board inside a computer. 

!(Uploading 463052447-9812e660-046c-4d30-9dd5-5468572b2cc7.jpeg…)
   
     Component           	Description
  
    CPU Socket.         	The slot where the processor (CPU) is installed

    RAM Slots (DIMM)   	Slots for installing memory modules (RAM)

    Chipset	              Manages data flow between CPU, memory, and peripherals
   
     BIOS/UEFI Chip	         Firmware that initializes hardware during boot-up

     Power Connectors	      Connectors for power supply to distribute electricity to components
     
     Expansion Slots.      	Slots (PCI, PCIe) for adding graphics cards, network cards, etc.

     SATA Ports	             Connectors for storage devices like HDDs and SSDs

     M.2 Slots	              Connectors for modern high-speed SSDs

     CMOS Battery	           Powers the BIOS memory to retain settings when the PC is off
 
      USB Headers          	Connectors for USB ports on the front or back panel
     
      Audio Connectors.     	Ports for audio input/output devices
     
     Network Port(Ethernet)  	Connector for wired network connections

  !(Uploading 463052447-9812e660-046c-4d30-9dd5-5468572b2cc7.jpeg…)

## 01/07/2025
  ## Common issues and Problems in PC:

### GPU (Graphics processor unit):
- Responsible for rendering graphics and visual output.
- Problems include overheating, driver issues, screen tearing, or no display output.

### PCU (Personal Computer Unit):
1. Installation & Hard Disk Preparation:<br>

* Partitioning: The first step of Partitinong is to organize the hard disk into:
  * **Primary (C: Drive):** <br>
    - Where the Operating System (Windows/Linux/Unix) is installed.
    - Avoid storing personal/important files in **C:**
      - If Windows crashes, files in D:, E:, F: are safer and can often be recovered.
  * **Logical Drives (D:, E:, F:):** Used for pictures, videos, documents, etc.

2. Speed slow (Causes & Fixes): <br>
-	Desktop: Files should be on drive. By default files on desktop are stored on C drive. As OS system is installed in C: file, its recomended to not put many folders in Desktop. Move them into drives. 

-	Task bar: Keep minimal shortcuts on the taskbar 

-	Browser (Bookmarks): Avoid excessive browser bookmarks as they slow down browser start-up.

-	Temporary files: These files are created by websites & cookies, and stored/ download in hidden files. Ulitmately because of it the system slows down.  So, after a period of time remove temporary files.

- RAM overuse: Don't open a number of applications or tabs are open at once. As ulitimately we are using the RAM.

-	Malware: Regularly scan your system for malwares.

-	Fragmentation: <br>
    There shouldn’t be chaos or dely to access files. <br>
    To make system efficient in working and get work done in optimal way, defragmentation is done.<br>
    * Go to `Start → Defragment and Optimize Drives`
    * Schedule defragmentation for automatic optimization.

4. Printer Issues & Solutions:
   
| Problem                            | Solution                                  |
| ---------------------------------- | ----------------------------------------- |
|  Paper Jam                       | Remove the stuck page carefully           |
|  Printer Out of Paper During Print Job | Use Queue.                 |
|  Faded or Poor Quality Prints   | Refill or replace ink/toner               |
|  Overlapping Lines in Print      | Possible **drum issue**, replace the drum |

###  Blue Screen of Death (BSOD):
It is used to indicate a system crash, in which the operating system reaches a critical condition where it can no longer operate safely.

**Common Causes of BSOD:**

1. Hardware Failures: <br>
   Faulty RAM, hard disk, or other internal components
2. Driver Issues: <br>
   Outdated, incompatible, or corrupted device drivers
4. Corrupted System Files: <br>
   System file corruption due to improper shutdowns, malware, or failed updates
5. Overheating or Power Issues: <br>
   Inadequate cooling or power supply malfunctions

###  System Crash Analysis:

After a BSOD, Windows creates a **dump file** that records what happened before the crash.

### Tools for Analysis:
1. **Event Viewer:** <br>
   Windows tool to check detailed system and crash logs.
2. **WinDbg:** <br>
   Microsoft Debugging Tool for analyzing dump files    |
   
### BIOS/UEFI Settings and POST Errors:

| BIOS                      | UEFI                                  |
| ------------------------- | ------------------------------------- |
| Basic Input/Output System | Unified Extensible Firmware Interface |
| Older firmware standard   | Modern replacement for BIOS           |
| Keyboard-only navigation  | Supports mouse and GUI                |
| Stored in ROM chip        | Stored in flash memory                |

BIOS/UEFI is responsible for initializing hardware components before the OS loads.


**What is POST?:** <br>
POST (Power-On Self Test) is a diagnostic process that occurs when the computer is powered on. It checks for:

* RAM functionality
* CPU status
* Keyboard presence
* Display detection
* Hard disk and drives

*Common POST Errors:*

| Beep Code / Message   | Meaning                                                   |
| --------------------- | --------------------------------------------------------- |
| 1 Long, 2 Short Beeps | Graphics card issue                                       |
| Continuous Beeps      | RAM failure                                               |
| No Beep, No Display   | Power or motherboard issue                                |
| “CMOS Checksum Error” | Corrupted BIOS settings (usually fixed by resetting CMOS) |

### Accessing BIOS/UEFI Settings

* Press **F2**, **F10**, **DEL**, or **ESC** continously during startup (key depends on manufacturer).
* From here, you can:

  * Change boot order
  * Enable/disable hardware components
  * View system info
  * Reset settings to default (if needed)

 
---
### Other small concepts: 

**Wizard-Based Installation:** <br>
GUI-based installation with no need to type commands.

**Antivirus Installation:** <br>
Essential for protection against viruses, malware, and spyware.

**Help Shortcut:**<br>
Press **F1** to open help tool in Windows.

## 02/07/2025
### Safe mode:
Safe Mode is a diagnostic mode in Windows that starts the computer with a minimal set of drivers and services, which makes it easier to find and remove harmful malware and viruses without activating them.

**Types of safe mode:** <br>
1. Safe Mode:<br>
   Used to diagnose and fix basic system issues.
   
2. Safe Mode with Networking: <br>
   Includes network drivers and services. Allowing access to the internet or network drives for troubleshooting.
   
4. Safe Mode with Command Prompt:<br>
   Loads a minimal environment with Command Prompt instead of the normal desktop interface
   
### Recovery tools:
- The Recovery Drive utility in Windows is a tool designed to back up essential system files needed to restore a PC to its original state.
- It fixes problems that prevent Windows from booting.
- Rolls back system files and settings to an earlier point in time without affecting personal files.

### OS repair:
It is used when the OS fails to boot or behaves abnormally.<br>
Use repair commands:
- sfc /scannow – Scans and restores system files.
- DISM /Online /Cleanup-Image /RestoreHealth – Repairs corrupted Windows images.
- Bootable USB for repair and system reinstall.

### Virus/Malware Symptoms:
- Slow performance
- Frequent crashes or freezes
- Slow startup
- Unexplained files or folders disappearing
- Unusual network activity:
  -  Malware can send or receive data, causing increased network activity, especially when your device is idle.
- Increased data usage:
  - Malware can consume more data than usual, especially if it's sending or receiving large amounts of information. 
- Browser-Related Symptoms:
  - Unwanted pop-up ads
  - Browser redirects
  
### Basic removal:
1.	Enter safe mode.
2.	Run Antivirus scan
3.	Delete suspicious Programs via Control Panel.
4.	Clear Temp files.
5.	Reset Web browser setting.
6.	Check startup Programs
7.	Update OS and antivirus.
   
### Where to Keep Windows Backups?
Backups are essential for recovery in case of OS failure or data loss.
- External Drive:
  Recommended option for offline, safe backup storage.
- Separate Internal Drive (e.g., D:, E:):
  Better than storing on the system drive (C:), but vulnerable if the whole disk fails.
- Cloud Storage:
  Services like Google Drive, OneDrive, or Dropbox allow automatic syncing and access from anywhere.

### Modern Internet Transmission (Wired Connections):
**RJ45**:
- RJ45 stands for Registered Jack 45.
- It is a standard connector used for Ethernet networking cables.
- RJ45 connectors are typically used to connect computers, routers, switches, and other networking devices.
- It has 8 pins (8P8C – 8 position, 8 contact) and connects twisted-pair cables like Cat5e, Cat6, Cat6a.
- Commonly used for LAN (Local Area Network) connections.

*Cat5, Cat6, Cat6e: Categories of twisted-pair cables used in wired networks, offering various speeds and shielding levels.*
## 04/07/2025
## How to Make a RJ‐45 Cable:
1. Strip the cable to remove 1 inch of the outer sheath.
2. Untwist and straighten the wires inside of the cable
3. Arrange the wires into the right order.

| **Pin Number** | **Wire Color (T568B)**   | **Signal**       |
| -------------- | ------------------------ | ---------------- |
| 1              | White Orange             | Transmit + (TX+) |
| 2              | Orange                   | Transmit – (TX–) |
| 3              | White Green              | Receive + (RX+)  |
| 4              | Blue                     | Unused / PoE +   |
| 5              | White Blue               | Unused / PoE +   |
| 6              | Green                    | Receive – (RX–)  |
| 7              | White Brown              | Unused / PoE –   |
| 8              | Brown                    | Unused / PoE –   |

4. Trim the wires into an even line 1⁄2 inch (13 mm) from sheathing
5. Insert the wires into the RJ-45 connector.
6. Stick the connector into the crimping part of the tool and squeeze twice.
7. Remove the cable from the tool and check that all of the pins are down & test the cable.

![](https://github.com/KamaljeetKaur00/Daily_bash_notes_2025/blob/main/images/RJ45-02.jpg)

## 07/07/2025
## **Introduction to HTML & Web Basics**

### HTML:
* HTML stands for HyperText Markup Language.
* It is the standard markup language for creating web pages and web applications.
* HTML defines the structure and content of a web page.

### **How browsers render it:**

1. The browser reads the HTML file line by line.
2. It builds the **DOM (Document Object Model)** — a tree-like structure of the page.
3. The browser then displays the structured content visually based on HTML + CSS.

###  Structure of an HTML Document
* `<!DOCTYPE>` declaration defines that this document is an HTML5 document
* `<html>` element is the root element of an HTML page
* `<head>` element contains meta information about the HTML page
* `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
* `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
* `<h1>` element defines a large heading
* `<p>` element defines a paragraph

![](https://github.com/Kamal-jeetkaur/Daily_bash_notes_2025/blob/main/images/html.jpg)

## 08/07/2025
## Introduction to HTML & Web Basics

### Common HTML Tags

**1. Headings:**

* Tags: `<h1>` to `<h6>`
* `<h1>` is the largest, `<h6>` the smallest
* Used to define titles or section headers

**2. Paragraphs:**

* Tag: `<p>`
* Used to define a block of text (paragraph)
* Automatically adds spacing before and after

**3. Lists:**

* **Ordered List**: `<ol>` for numbered lists

  * Each item inside: `<li>`
* **Unordered List**: `<ul>` for bullet-point lists

  * Each item inside: `<li>`

**4. Links:**

* Tag: `<a href="URL">link text</a>`
* Used to create clickable hyperlinks
* Can link to external sites, internal pages, or email addresses

**5. Images:**

* Tag: `<img src="image.jpg" alt="description">`
* `src`: source of the image
* `alt`: alternative text shown if image can't load

  ![](../images/BasicHtml.jpg)

  09/07/2025
  ## Introduction to HTML & Web Basics

### Forms and Input Types:

* Forms allow users to **enter and submit data** to a server or script
* Tag: `<form>` – wraps all input elements
* Common **input types**:

  * `<input type="text">` – single-line text field
  * `<input type="password">` – hides text for passwords
  * `<input type="email">` – for email input (validates format)
  * `<input type="number">` – numeric input only
  * `<input type="checkbox">` – select one or more options
  * `<input type="radio">` – select only one from a group
  * `<input type="submit">` – button to submit the form
  * `<textarea>` – for multi-line text
  * `<select>` – dropdown list of options

    ![](../images/formHtml.jpg)
    

### Semantic HTML:

Semantic tags describe **meaning and structure**, making code more readable and accessible:

* `<header>` – top section of a page or article (often includes logo or title)
* `<footer>` – bottom section (copyright, contact info, links)
* `<nav>` – navigation links/menu for the site
* `<section>` – groups related content within a page
* `<article>` – independent content (like a blog post or news item)

## 10/07/2025

## **Basic Styling Using CSS**

**1. Inline CSS:**

* Styling applied **directly inside an HTML tag** using the `style` attribute
* Example:

  ```html
  <p style="color: blue; font-size: 18px;">This is a styled paragraph.</p>
  ```

**2. Internal CSS:**

* CSS written inside a `<style>` tag within the `<head>` section of the HTML document
* Used to style the **whole page in one place**
* Example:

  ```html
  <head>
    <style>
      body {
        background-color: #f0f0f0;
        font-family: Arial, sans-serif;
      }
      h1 {
        color: darkgreen;
      }
    </style>
  </head>
  ```

## 11/07/2025
## Introduction to Git and Version Control:

### What is Git and Why Use Version Control

* **Git** is a **distributed version control system** used to track changes in source code during software development.
* It helps manage code across multiple versions, developers, and updates.
* **Version control** allows:

  * Tracking changes over time
  * Restoring previous versions of files
  * Collaboration among multiple developers without conflicts
  * Safe experimentation with new features

### Git Architecture

**1. Repository (Repo)**

* A **storage area** where Git tracks all file changes
* Can be:

  * **Local**: on your computer
  * **Remote**: on platforms like GitHub, GitLab

**2. Working Tree**

* The actual files and directories you're currently working on in your system
* Reflects the current state of your code
* You make changes in the working tree before committing them

**3. Index (Staging Area)**

* A **temporary area** where you add files before committing to the repo
* It allows you to prepare exactly what will go into the next commit
* Acts as a buffer between the working directory and the repository

![](https://d8it4huxumps7.cloudfront.net/uploads/images/6465f5b7125e4_what_is_git_1.jpg?d=2000x2000)


## How to use Git? (With Command Line)

1. Create a repository<br>
![](../images/Git1.jpg)

2. Copy the HTML line of the repo<br>
![](../images/Git2.jpg)

3. Go to Git Bash

4. Run command: `git clone link`

5. Check if you got the repo cloned on your local dive by `ls`

6. Move inside the direcotry by `cd repo_name`

7. Check the content inside your repo (optional)

8. Check status of the repo by `git status`
   * If the response id 'Up to date', you are good to move forward
![](../images/Git3.jpg)

9. Create a new file by `touch file_name.html`

10. Open the file by `nano file_name.html`, write your code and save it.<br>
![](../images/Git4.jpg)

11. Add by: `git add file_name.html`<br>
![](../images/Git5.jpg)

### Warning Explained:

> `warning: in the working copy of 'first.html', LF will be replaced by CRLF the next time Git touches it`
- Right now the file has Unix-style (`LF`) endings, but since im on Windows, Git may convert it to Windows-style (`CRLF`) later.
- It's **safe to ignore**

12. `git push origin main`:
    - It directs and you get asked to authorize Git Credential Manager, which securely saves GitHub login credentials for pushing/pulling code. <br>
   
    ![](../images/Git6.jpg)

    - Click on 'Authorize git-ecosystem'
      
    ![](../images/Git7.jpg)
    
    - Enter your password
      
    ![](../images/Git8.jpg)

 14. To commit: `git commit -m "message"`
     ![](../images/Git9.jpg)
     - I haven’t set a Git identity yet, so git commit cannot proceed.
     - To fix this run:
     - git config --global user.name "name"
     - git config --global user.email "your-email@example.com"<br>
       > **email should match your Github email, but its not necessary for `name`**<br>
 15. Try `git commit -m "message"` again, and push this by command: `git push origin main`:
           
       ![](../images/Git10.jpg)


17. Now you can see the file in your repo:
    ![](../images/Git11.jpg)

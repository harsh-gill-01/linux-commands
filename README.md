# COMPREHENSIVE GUIDE TO LINUX #

## WHAT IS LINUX? ##

**DEFINITION:**

* **Linux** is a highly secure, flexible, and **open-source operating system (OS)** originally based on the principles of Unix.

* **Open-Source**: This means the source code is completely open to the public. Anyone can freely view, modify, customize, use, and contribute to its ongoing development.

* **Operating System (OS)**: An OS acts as a core interface between the user and the computer hardware. It manages system resources, handles communication, and allows users to download, install, and run various software applications.

---

**EXAMPLES OF OPERATING SYSTEMS:**
 
* Apart from Linux, other widely used operating systems include **Microsoft Windows** and **Apple macOS**.

* *Fun Fact*: **Android** used in mobile phones is also internally powered by the **Linux kernel!**

---

**BACKGROUND & HISTORY OF LINUX:**

* **Linux** was created by a **Finnish** software engineer named **Linus Torvalds** in **1991**.

* The name "Linux" is a clever combination of the creator's name **Linus** and **Unix**.

* Linux is designed as a **Unix-like** operating system, built from scratch to mimic the behavior of Unix without using its proprietary code.

---

**WHAT IS UNIX?**

* **Unix** is a powerful, multi-user, and multitasking operating system originally developed in the **1970s** at **AT&T's Bell Labs**.

* It serves as the historical foundation and design inspiration for many modern operating systems.

* While Linux is not directly derived from Unix code, it follows the **Unix philosophy and architecture** closely. This is why Linux is universally described as being **"based on Unix"**.

---

**LINUX vs UNIX:**

* **Unix** is a proprietary (licensed) system, whereas **Linux** is completely free and open-source.

* Linux is inspired by Unix and designed to be **Unix-like**. It works on the same principles and standards, making it **work smoothly with** Unix software and commands.

* This is why Linux commands look very familiar and work exactly like Unix principles.

---

**LINUX IS NOT AN OS:** 

* We cannot use Linux directly because it is not a complete operating system on its own.

* Linux is actually just an open-source **KERNEL**.

---

**WHAT IS A KERNEL?**

* A **Kernel** is the heart or core part of an operating system.

* It acts as a bridge to manage system resources and handles all communication between the computer **hardware and software**.

---

**BRIEF EXAMPLE TO UNDERSTAND:**

* Think of the **Kernel** as a **car engine**. Every car needs an engine to run, and similarly, every operating system needs a kernel to function properly.

* So, the **Kernel is the engine** fitted inside various complete operating systems.

* In the tech industry, there are many different operating systems (called Linux Distributions or Distros) that are built using the exact same **Linux Kernel**.

---

**EXAMPLES OF LINUX DISTRIBUTIONS:**

* **Linux Ubuntu, Linux CentOS**, and **Linux RedHat** are popular examples of operating systems built using the Linux Kernel. These are universally known as **Linux Distributions** or simply **Distros**.

* These operating systems are completely powered by the core **Linux Kernel** (the main engine). So, we do not use the raw Linux kernel directly; instead, we use these complete Distros built around it.

---

**WHAT ARE LINUX DISTRIBUTIONS (DISTROS)?**

* A **Linux Distribution (Distro)** is a complete operating system created from a collection of software.

* It includes the core **Linux Kernel**, a graphical interface, various system utilities, and a **package management system** (like **`apt`**) to easily install, update, and manage software applications.

---

**KEY FEATURES OF LINUX:**

* **Open Source:** The source code is completely free and available to the public, allowing anyone to modify and customize it.

* **Multiuser:** Multiple users can access system resources and run applications simultaneously without affecting each other.

* **Multitasking:** The system can handle and execute multiple tasks or processes at the exact same time smoothly.

* **Security:** Provides strong, built-in security features, user permissions, and regular community updates to stay protected.

* **Portability:** Highly flexible and can run efficiently on various hardware platforms, from old laptops to massive cloud servers.

---

**MARKET DEMAND:**

* **Job Roles**: Linux skills are in massive demand for high-paying roles such as **System Administrators**, **DevOps Engineers**, **Cloud Architects**, **Software Developers**, **Network Engineers**, and **Cybersecurity Professionals**.

* **Industry Adoption**: Top tech giants like **Google**, **Meta (Facebook)**, and **Amazon**, as well as major financial institutions and healthcare providers, heavily rely on **Linux** to run their entire IT infrastructure.

---

**RECOMMENDATION FOR BEGINNERS:**

* **Ubuntu**: It is widely used, highly beginner-friendly, and has extensive documentation with a massive community for instant support.

* (**Note**: All the practical guides and live terminal examples in this bundle are fully tested on **Ubuntu**).

* **CentOS**: It is the popular community version of **Red Hat Enterprise Linux (RHEL)** and is commonly used in enterprise server environments.

---

**UNDERSTANDING VIRTUAL MACHINES (VMs)**

**WHAT IS A VIRTUAL MACHINE?**

* **Definition:** A Virtual Machine (VM) is a software-based computer that runs inside your actual physical computer. It acts exactly like a completely independent and separate computer system. Since it is made of software, you cannot physically touch it, but it works exactly like a real hardware computer.

* **Real-World Example:** On your laptop, **Windows or macOS** is your main physical operating system. But when you run another separate operating system inside it—like **Ubuntu Linux** that isolated secondary system is called a Virtual Machine.

* **How it Works:** It borrows a small part of your physical computer's resources—like a little bit of **RAM, CPU, and Hard Disk space** to run this separate operating system smoothly.

* **The Big Benefit:** You can install and run **Ubuntu Linux** or any other distro **(RedHat, Fedora, Mint, CentOS)** inside a VM. It is **100% safe**. Even if you run a wrong command or break something inside the Linux VM, your main Windows/macOS system will remain completely untouched and secure.


**VIRTUALIZATION EXPLAINED**

* **Understanding Cross-Platform Access:** Your physical laptop or computer is the main **hardware** resource. For example, if your system has **Microsoft Windows** installed by default, you do not need to delete it to use **Linux**. By using **virtualization technology**, Windows remains completely safe on your system while you seamlessly access and run your desired Linux environments like **Ubuntu, RedHat, or CentOS.**

* **Universal Compatibility (Not Just for Windows):** Virtualization is not restricted to **Windows** users. It is a **universal technology**. If you are using macOS, you can use virtualization to run Windows or Linux. Similarly, if your default operating system is Linux, you can easily host and access macOS or Windows environments inside it.

* **Multi-OS Management:** Virtualization allows you to securely access, set up, and run multiple operating systems simultaneously on a single piece of computer hardware.

* **The Layer Architecture:** Under the hood, virtualization acts as an intelligent software layer between your physical hardware and the multiple operating systems. It smoothly manages communication between different systems by efficiently dividing a single physical computer server into multiple independent virtual computers.

**UNDERSTANDING HYPERVISORS**

**What is it?:**

* A **Hypervisor** is a software layer that allows you to create and run Virtual Machines (VMs). It acts as a manager that helps you easily set up, create, and maintain different virtual environments on one computer.

**REAL-WORLD EXAMPLES:**

* **Popular Tools:** Free tools like **Oracle VirtualBox** and **VMware** are great examples of hypervisors. They help you run multiple operating systems at the same time by **dividing** your computer's main hardware into smaller, isolated VMs.

* **Easy Access:** You just need to install Oracle VirtualBox or VMware software on your computer, create a new VM, and you can easily access any other operating system without disturbing your main system.


**TYPES OF HYPERVISORS**

* Hypervisors are divided into two main categories depending on where they are installed and how they manage the hardware resources.

**1**. **TYPE-1 HYPERVISOR (Bare-Metal)**

* **How it works:** This hypervisor installs **directly on the computer's physical hardware.** It does not need a default operating system like Windows to run.

* **Where it is used:** Tech companies and cloud giants (like **AWS, Azure, and Google Cloud**) use Type-1 hypervisors in their massive data centers because they are incredibly fast, secure, and highly efficient.

* **Popular Examples: VMware ESXi, KVM,** and **Microsoft Hyper-V**.

**3**. **TYPE-2 HYPERVISOR (Hosted)**

* **How it works:** This hypervisor installs or hosts **on top of your existing operating system** (like a regular app on Windows or macOS) that is why it is called hosted.

* **Where it is used:** It is perfect for software developers and students for personal practice, testing new applications, and running a safe Linux sandbox on their regular laptops.

* **Popular Examples:** **Oracle VirtualBox** and **VMware Workstation**.

**NOTE:**

* The basic functionality of a **Bare-Metal Hypervisor** and a **Hosted Hypervisor** is the same. The only difference is that Bare-Metal installs directly on the physical computer hardware, while a Hosted hypervisor runs inside an existing operating system (like running Linux inside Windows).

**HOW DOES A HYPERVISOR WORK?**

* A hypervisor (like VirtualBox or VMware) dynamically borrows and shares the main hardware resources from your host operating system (the pre-installed OS on your laptop).

**AN EASY EXAMPLE:**

* Imagine you have a laptop with **8 GB RAM** and **100 GB Disk Space**. You install a hypervisor (VirtualBox) on it to run another operating system.

* The hypervisor will now divide your main hardware resources to create an isolated mini-computer inside your laptop. This mini-computer is called a **Virtual Machine (VM)**.

**RESOURCE DIVISION:**

* Suppose you create two different Virtual Machines (Linux and macOS) on your laptop. The hypervisor will divide your total resources like this:

* **VM 1 (LINUX):** Consumes **2 GB RAM** and **30 GB Disk Space** out of your total 8 GB RAM and 100 GB HDD.

* **VM 2 (macOS):** Consumes **3 GB RAM** and **30 GB Disk Space**.

* *Remaining for Main Windows:* Your main host laptop is left with **3 GB RAM** and **40 GB Disk Space** to run smoothly.

**WHY DO WE NEED TO CHOOSE AN OPERATING SYSTEM?**

* **OS Selection is Mandatory:** When you create a Virtual Machine, it acts exactly like real physical hardware. Just like a physical laptop cannot perform any work without an operating system (like Windows or macOS) installed on it, a VM also requires you to select and install an operating system (like **Ubuntu Linux**) to actually run applications and perform tasks.

**BENEFITS OF VIRTUAL MACHINES (VMs)**

* **Cost Efficiency:** You do not need to buy new physical hardware to try or use a different operating system. For example, you don't need to purchase an expensive Apple laptop just to test or use macOS features.

* **Zero Risk Sandbox:** There is absolutely no risk of causing any damage or errors to your primary operating system (your default pre-installed OS like Windows).

* **Safe Application Testing:** You can easily test any software or custom script on different operating systems in a completely isolated environment without touching your host machine.


**WHY DO COMPANIES USE VIRTUALIZATION?**

* In the corporate world and massive cloud data centers, virtualization is highly essential because it provides huge financial and operational advantages:

* **Cost Efficiency:** It is extremely cheap compared to buying multiple physical servers. Companies can run dozens of virtual environments on a single physical machine, saving massive amounts of money.

* **Resource Optimization:** It drastically reduces **physical space, energy consumption (electricity bills), and cooling costs** in data centers.

* **Reduced Workload:** Managing virtual infrastructure requires less manual effort, allowing IT teams to automate server setups and reduce overall operational workload.

* **Instant Backups via Snapshots:** Hypervisors allow administrators to take a **"Snapshot"** of a Virtual Machine. A snapshot freezes the exact active state of the system, acting as a quick backup point.

* **Easy Disaster Recovery:** If a virtual server crashes or encounters an error, companies can instantly restore it back to a healthy state using the saved snapshot within seconds.

**BONUS CONCEPT: WHAT IS A SNAPSHOT?**

* **The Save-Game Layout:** A **Snapshot** acts exactly like a "Save Game" button for your Virtual Machine. It captures and freezes the exact state, files, and memory of your Linux system at a specific moment.

* **The Ultimate Safety Net:** Before performing risky operations or editing system files (like **`.bashrc`**), you take a snapshot. If a wrong command completely crashes or breaks your Linux system, you can press **`Restore`** to bring your system back to that healthy point in just 5 seconds, avoiding a full reinstallation.


**HOW LARGE COMPANIES USE SNAPSHOTS IN REAL LIFE**

* In big IT companies and cloud data centers, engineers use snapshots every day for these simple reasons:

* **1**. **Safe Software Updates:** Before updating any software or app on a live company server, engineers always take a snapshot. If the new update crashes the website or causes an error, they instantly restore the clean snapshot. This keeps the website running without disturbing the users.

* **2**. **Fresh Testing Environments:** Testing teams need a clean computer to test apps. After testing an app (which creates a lot of junk files), they simply restore the virtual machine back to its original snapshot. This gives them a fresh, clean system for the next test instantly.

* **3**. **Cyber Security Defense:** When a company installs a new security patch to block hackers, they take a snapshot first. Also, if a test computer accidentally gets infected with a virus, engineers do not waste time cleaning it. They just reset the computer to a healthy snapshot in 5 seconds.


**MASTERING THE VIM EDITOR**

**WHAT IS VIM?**

* **Core Definition:** Vim (Vi Improved) is a highly powerful, text-based file editor used in **Linux** environments. It helps a lot whenever you need to create, view, or modify files.

* **The Upgraded Tool:** There are other editors in Linux like **Vi** and **Nano**. Nano is very beginner-friendly, while Vi is the classic editor. Vim is the upgraded version of Vi, packed with new features and advanced functions. It requires a little bit of knowledge to operate, but it turns you into a pro user.

---

**HOW TO CHECK AND INSTALL VIM?**

If you want to check whether Vim is already installed on your system or you want to install it from scratch, use the following simple terminal commands:

---

**1**. **Check if Vim is Installed:**

To verify if Vim is present on your machine, run this command:

```bash
`which vim`
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/0de12243-68f0-4593-88bd-ac75c0eb6901" />

---

**2**. **Install Vim (If not present):**
 
If the previous command shows no path, you can easily install the Vim editor on your Ubuntu/Debian system by running:

```bash
sudo apt install vim
```

---

**HOW TO RUN VIM FROM THE TERMINAL?**

* To open the Vim editor directly without creating or opening a specific file, simply type the following command in your terminal and press **`Enter`**:

```bash
vim
```
---

**EXPECTED OUTPUT: THE VIM WELCOME SCREEN**

* When you execute the raw **`vim`** command, you will be greeted by the official Vim welcome and information dashboard inside your terminal screen:

<img width="400" alt="image" src="https://github.com/user-attachments/assets/194b5f11-1c61-43be-a404-6c1694f49e7a" />

**KEY DETAILS DISPLAYED ON THE SCREEN:**

* **Version Info:** Shows the current version of the editor (e.g., **Vim version 9.1**).

* **Core Shortcut Tip:** The screen itself helps beginners by displaying the most important command to close the editor: type **`:q`** and press **`Enter`** to exit.

---

**CREATING AND EDITING A NEW FILE**

* To create a completely new file or open an existing file for editing, enter the **`vim`** command followed by your desired filename.

**SYNTAX:**

`vim <file_name>`

**EXAMPLE:**

`vim new_file`

```bash
vim new_file
```

---

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/da9588c2-54ff-4cce-9d13-d72c0bd12496" />

---

**INSIDE THE VIM EDITOR WINDOW**

* Once you press **`Enter`**, Vim will switch to the editor screen where you can perform all your text editing operations.

* **File Status Indicator:** If you created a brand new file, you will immediately see your filename followed by a **`[New]`** tag at the very bottom-left corner of the screen (e.g., **`"new_file" [New]`**). This confirms that the file is fresh and empty.

<img width="400" alt="image" src="https://github.com/user-attachments/assets/8f9534b4-c19e-41bd-8cd7-fcdce7d9183f" />

---

**HOW TO START WRITING IN VIM (INSERT MODE)**

* **The Default State:** When you open Vim, you cannot start writing or typing text directly. You are inside the **Normal Mode** by default.

* **Switching to Insert Mode:** To start editing or writing code, you must first press the small **`i`** key on your keyboard.

* **The Indicator:** Once pressed, the status line at the very bottom-left corner will display **`-- INSERT --`**, confirming you are now in the typing mode.

---

**EXPECTED OUTPUT: INSERT MODE**

* Once you press the shortcut key, the terminal will dynamically display the mode transition at the very bottom:

<img width="400" alt="image" src="https://github.com/user-attachments/assets/e9c8f46c-f723-436a-9a6b-6329116ed53c" />

**SHORTCUT ACTION:**

* **`i`** — Press this key to switch from Normal Mode to Insert Mode to start editing or writing your text.

```bash
i
```

---

**HOW TO SAVE AND EXIT VIM**

* Once you have finished writing or editing your file, you must return to the terminal by safely saving your changes. Follow these precise steps:

**1**. **Exit Insert Mode:**

• First, press the **`ESC`** key on your keyboard. This will instantly remove the **`-- INSERT --`** tag and take you back to **Normal Mode**.

**2**. Save and Close Command:

• Type a colon **(`:`)** and then type **`wq`** (which stands for **W**rite and **Q**uit), then press **`Enter`**.

**KEYBOARD SHORTCUTS:**

* **`ESC`** — Leave **`-- INSERT --`** mode and go back to Normal Mode.

* **`:wq`** — Save your changes and exit the editor.

---

**EXPECTED OUTPUT: RETURN TO NORMAL MODE**

* When you press the **`ESC`** key, the **`-- INSERT --`** indicator will instantly disappear from the bottom-left corner of your screen, as shown below. This confirms that you have successfully left the typing mode and returned to **Normal Mode**.

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ef930f7e-8a5a-44d0-a461-11bb67417111" />

---

**EXPECTED OUTPUT: EXECUTING THE SAVE COMMAND**

* After returning to Normal Mode, type a colon **(`:`)** followed by **`wq`**. You will see the command appear at the very bottom-left corner of the screen, exactly as shown below. Now, press **`Enter`** to save your work and safely exit back to your main terminal window.

<img width="400" alt="image" src="https://github.com/user-attachments/assets/0c79842f-4ca2-42a8-a9d0-4f5a4f1f9c5d" />

---

**EXPECTED OUTPUT: VERIFYING THE SAVED FILE**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/53b1bd4f-29ef-4077-bb19-05bab428112f" />

* After executing the save command, you will immediately return to your main terminal screen. You can now verify that your file was successfully saved and created by using the following commands:

**1**. **Check if the file exists:**

```bash
ls
```

As shown in the output, **`new_file`** is now visibly present inside your directory.

**2**. **View the saved content inside the file:**

```bash
cat new_file
```

**EMERGENCY FIX: HOW TO QUIT WITHOUT SAVING?**

* **The Problem:** If you open a configuration file by mistake and accidentally type something incorrect or unnecessary, you do not want to save those broken changes.

* **The Solution:** You can force-close the editor immediately without saving anything by running the force-quit command.

**STEPS TO FORCE QUIT:**

**1**. Press the **`ESC`** key to leave Insert Mode and return to Normal Mode.

**2**. Type a colon **(`:`)** followed by **`q!`** (which stands for **Q**uit immediately with an exclamation mark to force the action), then press **`Enter`**.

**KEYBOARD SHORTCUT:**

`:q!`

**EXPECTED OUTPUT: FORCE QUITTING IN ACTION**

**1**. **Simulating an Accidental Edit:**

* Suppose you accidentally type a string of incorrect characters (like **`abchsodhslfn`**) inside your file. To discard this change, press **`ESC`**, type **`:q!`**, and hit **`Enter`**.

<img width="400" alt="image" src="https://github.com/user-attachments/assets/a69bc8df-63ac-4e33-ade7-2f156b70e0b1" />


**2**. **Verifying the Rollback:**

* Once you are back in the main terminal, execute the **`cat`** command to view the file contents. As shown in the output, the corrupted text was successfully discarded, and only your original healthy text remains:

```bash
cat new_file
```

<img width="400" alt="image" src="https://github.com/user-attachments/assets/1b97c4f2-a499-4cdb-8fe1-19fe9a59c273" />

---

# Linux Commands #

## My Linux Commands And Bash Scripts Notes ##

* **`ls`** - To **list all the contents** (files and folders) of our **current directory**.

```bash
ls
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/be73df06-9236-432f-9fa1-e12a1ee15256" />

---

* **`pwd`** - To **check which directory or location** we are **currently working in**.

```bash
pwd
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ff1b54b0-3440-41a6-b55b-320d0baead12" />

---

* **`clear`** - To clear **our terminal screen**. You can also use **`CTRL + L`** to **clear your terminal faster** than typing **`clear`** command.

**DIFFERENCE:**

* **`clear` command**: It **clears the terminal screen** by pushing your previous terminal work upward. If you **scroll up**, you can still see your previous commands and output logs.

* **`CTRL + L` shortcut**: This is an **instant keyboard shortcut**. It does the same job rapidly without requiring you to type anything, helping you **work much faster**.

```bash
clear
```

**EXPECTED OUTPUT (`clear` command):** 

<img width="400" alt="image" src="https://github.com/user-attachments/assets/c0f237ca-438d-4ad2-8515-e07cb842b0c6" />

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ff21990b-b45d-4f31-89c9-29f4394134ce" />

---

* **`date`** - To **check the current date**, along with the **exact time and timezone**.
  
```bash
date
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ba21578d-6138-46fb-853f-be55d65f16d5" />

---

* **`touch`** - To **create an empty file** in Linux.

**SYNTAX:**

* `touch [file_name]` 

**EXAMPLE:**

* `touch my_file`

```bash
touch my_file
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/4d1d143b-53d9-451d-92b8-2135d3469925" />

---

* **`mkdir`** - To **create a new folder** (directory) in Linux.

**SYNTAX:**

* `mkdir [folder_name]` 

**EXAMPLE:**

* `mkdir my_folder`
 
```bash
mkdir my_folder
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/6ef15c28-a0c7-41f3-a9c2-41a8b09342e0" />

---

* **`rm`** - To **delete a file** in Linux.
  
**SYNTAX:**
  
* `rm [file_name]` 

**EXAMPLE:**

* `rm my_file`

```bash
 rm my_file
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/35679bfb-04c4-4e3b-b5cd-f4e85d9fc905" />

---

* **`rm -rf`** - To **delete a folder** (directory) in Linux. You can also use the **`rmdir`** command for the same purpose, but `rmdir` only works on empty folders, while `rm -rf` can **force-delete any folder along with its hidden contents**.


**SYNTAX:**

* `rm -rf [folder_name]`

**EXAMPLE:**

* `rm -rf my_folder`

```bash
rm -rf my_folder
```

**SYNTAX:**

`rmdir [folder_name]` 

**EXAMPLE:**

`rmdir newfolder`

```bash
rmdir newfolder
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/6c50249e-afd1-4158-a3f6-4d4a2385aa5e" />

---

* **`cal`** - To **see the calendar** of the current year or month. We can also **see calendars of past or future years** along with specific months by writing the year number and month number.

```bash
cal
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/75decda2-4326-43f7-a0a6-0c27c9ce8374" />

---

* **`ls -l`** - To **list all the contents** of a directory in the **long listing format**. It shows deep details like **file permissions, owner name, file size, and the exact date and time** the file was created or edited.

```bash
ls -l
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/20d7ca50-491a-4922-9b05-7425ff7a80c3" />

* You can also use **`ls -l <file_name>`** for **finding and getting information** about **only one file** (including hidden details).

**SYNTAX:**

* `ls -l <file_name>`

**EXAMPLE:**

* `ls -l file_A`

```bash
ls -l file_A
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/52d94319-8628-4a45-b06c-f204d2545846" />

---

* **`ls -lt`** - To **list all contents** sorted by **time and date** (newest files appear first at the top).

```bash
ls -lt
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/7050b9ef-214a-4b10-9d66-7c55d80cff30" />

**NOTE:**

* In the screenshot, you can clearly see the **sorted date and time**, along with the names of the files that are **newly created or modified**.

---

* **`ls -ltr`** - To **list all contents** sorted by **time and date in reverse order** (newest files appear at the very bottom, making them easy to see without scrolling up).

```bash
ls -ltr
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/24a9ca76-d0be-493d-90a4-4a47e32cc3fc" />

**NOTE:**

* In the screenshot, You can clearly see the **newest files are appearing at the very bottom**.

---

* **`ls -lh`** - To **see information about our files and folders** in a manner that makes them **much easier to read**. In this command, **`h`** means **human readable**.


```bash
ls -lh
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/f680aa0c-26fc-4c5f-832f-6dfd9cbe2c55" />

**NOTE:**

* You can clearly see that the **file sizes have changed into a human readable format**.

* You can **check other helpful flags and options** of `ls` by using the **`ls --help`** command.

```bash
ls --help
```

---

* **`bc`** - To **open a calculator-like system** in your terminal to do **basic calculations**. Generally, you will not get a visual calculator window. Instead, you will get a **clean platform inside your terminal** to perform mathematical equations. Press **`CTRL + D`** to exit the calculator and come back to your main terminal screen.
 
```bash
bc  
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/552a061d-745f-48af-8a8a-0532db518221" />

---

* **`--help`** - To **get help regarding any specific command**. You will write the main command first, followed by this help flag, to see all available options.

**SYNTAX:**
  
* `<command_name> --help` 

**EXAMPLE:**

* `ls --help` 

```bash
ls --help
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/24dd95f5-3a79-45d7-a280-ac82d06b64a0" />

---

* **`man`** - To **get the official manual** regarding any specific command. This command helps you by **providing full detailed information** about its uses, options, syntax, and real-world use cases. Press **`q`** to exit the manual screen and come back to your terminal window.

**EXAMPLE:**

* `man ls`

```bash
man ls
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/121c2e92-1727-4c92-b243-7b585fa03f68" />

---

* **`cd`** - Use this command to **change directory** or for surfing in multiple folders and directories . You can also use **`/`** for going or moving in multiple folders by describing path. This command will let you **access directories of current location**.Always remember to give the exact name of the folder you want to open. If you use this command alone (without typing any folder name), **it will instantly bring you back to your home directory (`~`)**. Note that directories and folders appear in a different color on the terminal.


**SYNTAX:**

* `cd [folder_or_directory name]`

**EXAMPLE:**  

* `cd folder`

```bash
cd folder
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/fc7fa4bb-0b3c-43d2-8db0-03a85c31e485" />

---

* **`whoami`** - To **know who you are** in this terminal. When you use this command, it will **return your username** through which you are logged in and working. The **`id`** command will **return other user identity details** like your user ID (**uid**), group ID (**gid**), and user groups.


```bash
whoami
```

```bash
id
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/8c596326-7135-4241-8bac-efb0f41bf657" />

---

* **`uptime`** - Use this command to **check how many users** are currently logged in, the **exact time duration** for which the terminal/system has been running, and the **current system load average**.
 
```bash
uptime
```

**EXPECTED OUTPUT:** 

<img width="400" alt="image" src="https://github.com/user-attachments/assets/35204fe9-0a3d-4811-b6ab-708bcdb1d4a3" />

---

* **`cd ../`** - Use this command to **go back one directory** from current location. You can use multiple slashes as per the number of folders or directories you are in to go back. In the **Expected Output**, i went to `folder` , then `newfolder` , then i went back one folder by using `cd ../` , then i went two folders back by `cd ../../` command , then i went upto `folderA` by describing its path from **home folder** .

**SYNTAX & OPTIONS:**

* `cd [folder_name]` - To **go inside a folder**.

* `cd ../` - To **go back one directory**.

* `cd ../../` - To **go back two directories**.

* `cd /foldername/foldername/foldername/` - By **describing path between slashes**, you can access your required folder.

**EXAMPLE:**

* `cd folder`

* `cd newfolder`

* ` cd ../`

* `cd ../../`

* `cd folder/newfolder/folderA`
 
```bash
cd folder
```
```bash
cd newfolder
```
```bash
cd ../
```
```bash
cd ../../
```
```bash
cd folder/newfolder/folderA
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/43305944-3f0c-495f-9a74-8b5f279e0c39" />

---

* **`mv`** - To move **files and folders** from one directory to another in Linux. We should give the exact name of the files and folders which we want to move. It moves them to the desired destination directory. You can also use this command to **change the name of files and folders** (rename them). We can also use the **`mv ../[file_or_folder_name]`** command to pull any folder or file into our current directory without manually going back.


**SYNTAX & OPTIONS:**

* `mv [file_name] [folder_or_directory]`.

* `mv [folder_or_directory_name] [folder_or_directory_name]`.
  
* `mv ../[file_or_folder_name] .` - You can **get any file or folder from any previous folders or directories** without going back by using the required number of `../` based on the location of files and folder.
  
* `mv [old_file or folder name] [new_file or folder_name]` -for **changing the name** of a file or folder.

**EXAMPLE:**

* `mv fileB my_folder`

* `mv folder mynewfolder` 

* `mv ../filenew .`

* `mv file_A file_AA`

* `mv folder FOLDER`

```bash
mv fileB my_folder
```
```bash
mv folder mynewfolder
```
```bash 
mv ../filenew .
```
```bash
mv file_A file_AA
```
```bash
mv folder FOLDER
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/eba6ae55-e775-4f90-824f-ec954a4d56d3" />

---

* **`cp`** - To **copy files and their contents** in Linux. The name of the source file should be written right after the command, followed by the destination folder or target file.

**SYNTAX & OPTIONS:**

* `cp [file_name] [folder or directory]`.

* `cp [file_name] [another file_name]` - For **copying only content** of one file to another file.

* `cp ../[file_name] .` - You can **get any file and its content from any previous folders** or directories without going back by using number of `../` as per the location of files or folders.

* `cp [file_name] [file_name]` - For copying the content as well as **creating new copy of file** with a different name.

**EXAMPLE:**

* `cp FILE new_folder`

* `cp FILE file_new`

* `cp ../fileC .`

* `cp file_new new_File`

```bash
cp FILE new_folder
```
```bash
cp FILE file_new
```
```bash
cp ../fileC .
```
```bash
cp file_new new_File
```

**EXPECTED OUTPUT:**

**FIRST TWO COMMANDS:** 

<img width="400" alt="Screenshot 2026-09-13 120616" src="https://github.com/user-attachments/assets/019ded80-8a35-471e-a5be-bbcfa9d61e5f" />

**LAST TWO COMMANDS**:

<img width="400" alt="Screenshot 2026-09-13 121310" src="https://github.com/user-attachments/assets/88e72df8-29f9-4a50-b6b8-33de27e63e92" />

---

* **`cat`** - To **read and view the content** of a file directly inside the terminal.

**SYNTAX:**

* `cat [file_name]`

**EXAMPLE:**

* `cat FILE`
   
```bash
cat FILE
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/e0eb7c18-fea6-4a1e-84bb-379bd1d71796" />

---

* **`less`** - To **read large files** comfortably. It provides better features than the `cat` command, allowing you to scroll through text and **search for specific words** easily. Instead of filling all your terminal screen, it opens the file in a **temporary full-screen reader view inside the terminal**. Press **`q`** to quit this view and return to your clean terminal.


**SYNTAX:**

* `less [file_name]`

**EXAMPLE:**

* `less file`

* `less fileB`

```bash
less file
```
```bash
less fileB
```

**EXPECTED OUTPUT:**

**Output of Smaller File (file):**

<img width="400" alt="Screenshot 2026-09-14 124048" src="https://github.com/user-attachments/assets/5e83c81d-388a-4977-ad3e-3f022e631394" />

**Execution of Bigger File (fileB):**

<img width="400" alt="Screenshot 2026-09-14 124404" src="https://github.com/user-attachments/assets/3fdd1856-cb9f-414e-90c9-6592bdff44a0" />

**Output of Bigger File (fileB):**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/84e2ac39-7acf-4c39-9d32-4c14a3933996" />

**NOTE:**

* **`/`** & **`?`** **for Searching:** Press `/` to search text from **top to bottom**, press `?` to search from **bottom to top**, and press `n` to find the next match until it shows **`Pattern not found`** (it will come written at the very bottom when there will be no another match).

* **Navigation Keys:** Press **`SHIFT + G`** to instantly go down to the **last line of the file**, and press `P` to jump back up to the **first line**.

* **Easy Exit:** Press `q` anytime to instantly **quit file reading** and come back to your clean terminal screen.

* **Interface:** This command opens your big files in a **temporary full-screen reader view** inside the terminal instead of filling all your normal command history.

**This Is How You Will Search specific information with `/` `?`:**

<img width="400" alt="Screenshot 2026-09-14 124546" src="https://github.com/user-attachments/assets/8779c41a-b356-422e-937b-e14a9ac08fb7" />

<img width="400" alt="Screenshot 2026-09-14 124631" src="https://github.com/user-attachments/assets/5cb522c6-265a-4b9a-8bd9-96fbbbe88dbc" /> 

---

* **`more`** - To **read a file page by page** or line by line. Press **`ENTER`** to scroll line by line, and press the **`Down Arrow`** from the keyboard to scroll page by page. It also shows the **exact percentage of the file you have read** at the bottom of the terminal screen. Press `q` to quit **file reading**.


**SYNTAX:**

* `more [file_name]`

**EXAMPLE:**

* `more fileC`

* `more fileB`

```bash
more filec
```
```bash
more fileB
```

**EXPECTED OUTPUT:**

**Output of Smaller File (fileC):**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ffd5900e-f2eb-44e4-bf0e-175fea7ed90a" />

**Execution of Bigger File (fileB):**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/2b02a7c4-96e6-49c9-b98e-9ef89c6166c1" />

**Output of Bigger File (fileB):**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/cd960e68-86d9-4375-a826-c1048128c7b6" />

**NOTE:**

* **File Opening Rule:** This command opens the file **inside your terminal**, not in a separate reader window like the `less` command.
  
* **File Size Requirement:** This page-by-page reading method will **only work on big files** and will not execute on small text files as usual, as you can see in one of the screenshots.

---

* **`nano`** - To **create and edit text files** very easily inside the terminal. It provides a built-in text editor platform where you can directly start typing your notes or code. If the file name you enter does not exist, `nano` will **automatically create a brand new file** for you.


**SYNTAX:**

* `nano <file_name>`

**EXAMPLE:**

* `nano fileB`

```bash
nano fileB
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/b4bb1cf4-0d0b-49ba-9c35-c42a38751af8" />

**NOTE:**

* Check my **dedicated nano editor guide** for more information, useful tricks, and to edit files like a pro.

---

* **`vim`** - To **edit files inside the terminal**. It is the **upgraded version of the traditional `vi` editor** and provides much better functions, though the basic core working is identical for both. It opens a highly powerful terminal-based file editor platform.

**SYNTAX:**

* `vim <file_name>`

**EXAMPLE:**

* `vim myfile`

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/16fee3e4-2baa-42bd-bbc5-0cf578909b9d" />

**NOTE:**

* Check my **dedicated vim editor guide** for more information and useful tricks to edit like a pro. You **cannot directly type text in the `vim`/`vi` editor** upon opening and you might face configuration errors if you do not know the modes. If you want a deep dive into `nano` or `vim` editors, please check our separate comprehensive manuals; the info provided here is a quick reference layout.

---

* **`grep`** - Its full form is **Global Regular Expression Print**. It is used to **search for specific words or patterns inside files**. It will search the text and instantly return all the lines containing that specific word on your terminal screen.

**SYNTAX:**

* `grep 'word' [file_name]`

**EXAMPLE:**

* `grep 'A' fileB`

```bash
grep 'A' fileB
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/d4977845-fcfb-4e35-b8e0-c805ea63e914" />

---

* **`egrep`** - To **search for multiple words and patterns** inside files at the same time. Write the name of the file and use the **pipe or vertical bar (`|`)** symbol to separate and search multiple target words at once. It will **highlight** all the searched words.


**SYNTAX:**

* `egrep 'word1|word2|word3' [file_name]`

**EXAMPLE:**

* `egrep 'A|G|H|J|C' my_file`

```bash
egrep 'A|G|H|J|C' my_file
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/7786c024-df89-4096-ae2c-1558449cd580" />

---

* `history` - Use this command get all the history of your used commands on terminal, use `history` command for getting all the commands history that are executed on the terminal till date. You can use `history |grep` command also to search a specific or single command name that you have executed on your terminal. The word `grep` is used here because it is used for searching words.
**Syntax:**
`history`
`history `|` [word or command]`

**Example:**
`history`
`history |grep ls`
 
```bash
history
history |grep ls
```
**Expected Output:**
Output of `History` Command
<img width="893" height="815" alt="image" src="https://github.com/user-attachments/assets/5b2fa1e2-ffae-4081-8d70-388710e26b92" />
Execution of `History |grep ' ' ` Command
<img width="890" height="78" alt="image" src="https://github.com/user-attachments/assets/3d17d75c-ce23-4306-a6e4-cc1b93f2cd0e" />
Output of `History |grep ' ' ` Command
<img width="888" height="814" alt="image" src="https://github.com/user-attachments/assets/ae1a2dd2-aeec-4ddf-956f-7aebf194811b" />

---

* `gzip -k` - Use this command to zip a file. It will compress your file and will give you the compressed version of your big file , thus helping us to share or store them easily.
 
**NOTE:**

You can also use `gzip` but, it will not give you real file along with compressed version, but `gzip -k` will, as it's `-k` describes that, keep input files, do not delete them. If you want to keep it's real file then use `gzip -k` and if not, then `gzip`. Use `gunzip -d` or `gzip -d` where `d` stands for decompress, for decompressing real file, when you use `gzip` and want to get back real file. Write the name of the file you want to compress or decompress. While decompressing the file , write name of your compressed version file ( .gz , at the end ). The compressed version file appears RED in color usually.

**Syntax:**
`gzip [file name]`
`gzip -k [file name]` (for keeping real file also)
`gzip -d` [compressed file name] (when you use `gzip`)
`gunzip -d [file name]` (one more command for decompressing,when you use `gzip` )



```bash
gzip new_file
gunzip new_file.gz
```
* `sort` - use this command to sort your unsorted file contents. Example - think of this you have , a file with letters a-z but they are mix, means unordered then, you can use `sort` command to set them in order from a-z in ordered form. use `sort -r` command to reverse the contents after sorting them in correct manner.
```bash
sort fileA
sort -r fileA
```
* `sort |uniq` - use this command to sort the contents of your file, but also to remove copy contents . Example - Think of this you have, a file in which you have a data of workers of a company, there can be multiple workers of name. Then , you can use `sort |uniq` command to sort that file along with removing copied or matched names to see some specific information.
```bash
sort filename|uniq
**syntax**
sort /filename|uniq
```
* `wc -l` - use this command to check how many lines of content or information a file contains. Write the name of the file of which you want to get number of lines.
 ```bash
wc -l file.txt
```
* `split` -l - use this command to split a big file in number of files as per your requirement and number of lines in that specific file. Example - Think of it you have, a file containing 20 lines or more and less, then you can split it into specific number of parts of files as per your choice and work. you can divide or split it into 2 split files or more. Give the number and after the command `split -l` .
```bash
split -l 3 my_file
```
* `alias` - use this command to get relief from writing long command in you terminal. This command is like a small hack for long command , you can use this command for normal use also like for short commands. Example - if you do not want to write even `ls` command again and again on your terminal, then you alias it like this `alias l= ls` or may be replace with other word `alias c= ls`. You can use this command as per your choice and comfort . Now when you will press or type l or c instead of full command , it will show you output of your edited command. Its temporary thing.
```bash
**syntax**
alias /the word or letter= command
alias l= ls -ltr
```
* `cmp` - to compare files means that, their content . Write the names of the files you want to compare. 
```bash
cmp fileA fileB
```
* `diff` - to see what is the difference between two files after comparing. Write the names of the files. Use `diff -u` command to get difference between two files more acurately with more information.
```bash
diff fileA fileB
diff -u fileA fileB
```
* `which` - this is used to check executables. Executables means the things that can be executed , means commands in linux or any other os terminal that we execute in the terminal to perform our work. Example - think of the command `ls` , we are able to execute only in the terminal if it is installed. When we do our work in terminal we can check the command if it is installed or not. Use this to check if a command that you are going to execute is installed or not.
```bash
which ls
**output**
usr/bin/ls
```
* `zip` - this command is used to zip or compress multiple numbers of files at same time.
This command helps us to zip and compress mutiple files.
```bash
zip myfiles.zip fileA fileB fileC fileD
**syntax**
zip / give here a name for zipped files.zip files names
```
* `unzip` - use this command to unzip multiple files. It will unzip all the files present in one zipped file. Use this command to unzip files, and this `unzip -l` command to see only some information about files stored in single big file, like, their date , time, names, numbers .
Use `unzip` to zip them and `unzip -l` to see only the information without unzipping them.
```bash
unzip myfiles.zip
unzip -l myfiles.zip
```
* `tar -czf` - this command is used to compress folders in linux. The word `-c` stands for compress.
```bash
tar -czf myfolder.tar.gz folder
**syntax**
tar -czf /give a name to your compressed folder.tar.gz /real folder name
```
* `tar -xzf` - this command is used to decompress the folder. The word `-x` means extract or decompress folder.
```bash
tar -xzf compress.tar.gz my_folder
```
* `find ./` - this command is used to find files. This is helpful because we can have a number of files in different folders or directories and we can not remember all of them. Path means, that, where it is located, in which folder it is. Example - think of this, that you have a file named File.txt , but you do not know where it is then you can use `find ./` command or even wildcard `*`(`find file*`) or (`find *txt`).Just remember that `find` command will find files for you when you will enter proper file name, but by using wildcards, you can find a file easily without knowing its full name. There are many ways to find files. You can use wildcards and `find ./` command like these in different ways - find./name newfile, find./*.txt, find file, find./ file, find file* .
```bash
**syntax**
find ./ -name (name of file)
```
* `script` - use this command to turn on script mode in your terminal. Use this command while you have to write something that you are going to see or execute commands again. You can use this command to save your work , if you are a beginner. All the work or commands that you will run after executing script command will get save in a file named TYPESCRIPT.
```bash
script
```
* `wget` - use this command to download files from internet. Write the URL_of_file or application you want to download. Example - if you want to download python, then you will copy its url from its website and will paste after the `wget` command. You can change the name of your file i.e python file by using `wget -o`. This is because it will be saved by its default name at first. But, you can change its name for sure.
```bash
wget
**syntax**
wget URL_of_file (for downloading file)
wget -o opt_file.txt URL_of_file (for changing name of file)
```
* `locate` - use this command to find or locate a file. This command takes out the file for you from database instead of from directories or folders. You have to use another command `updatedb` also. Example- you created a new file and you forgot in which directory or folder you made or put it, then you can use locate command to find it, but you have to use `updatedb` command because, it will take out file from database and if you did not update your database locate command will not work, so update your database before using locate command, because it does not take out fresh(new) created command.  Use `sudo updatedb` for ubuntu linux OS. Fill your password and update it.
```bash
locate 
```
```bash
updatedb 
```
* `apt` - use this command to install applications or packages in linux ubuntu. This command is for ubuntu. If you are using fedora, centOS , redhat then use `yum` or `dnf` commands for installation works. You have to use `sudo` command while installing something along with apt together , because installation requires root accesses and therefore we use root user `sudo` command. But , first try to install without using `sudo`. Use `sudo apt install <software or package name>` for installing. `sudo apt remove <software or package name>` for removing them. And , `sudo apt update` to update them and get latest versions or updates. `sudo apt upgrade`
```bash
sudo apt install
```
```bash
sudo apt update
```
```bash
sudo apt upgarde
```
```bash
sudo apt remove 
```
* `dpkg -l` - use this command to check packages or applications, if they are installed or not before using and after installing. This is .deb (debian) package of linux for managing its packages . It works for the offline files that you downloaded and want to manage them and see them if they are installed or not. Use `dpkg -l | less` command to check all the packages easily, as because using `dpkg -l` alone will scroll up all the information if there are a lot of packages and applications. But, you can also use this as your requirement.
 ```bash
dpkg -l | grep <file, application or package name> 
```
<img width="956" height="930" alt="image" src="https://github.com/user-attachments/assets/55da7397-235d-48cb-9b59-e5ceb612bbe2" />

```bash
dpkg -l | less <img width="971" height="937" alt="image" src="https://github.com/user-attachments/assets/153ff40a-d0cd-4904-a8bf-f340ed10c055" />
```
```bash
dpkg -l <img width="982" height="1008" alt="image" src="https://github.com/user-attachments/assets/bbbc97c0-d7eb-4f19-9ef5-f5e9e62b8080" />
```
* 'head -n' - use this command to read files in linux. This command will help you read specific number of upper lines in a file. For example - you have a file containing 100 lines, but you want to read only top 20 lines then you can use `head -n` command and by executing this `head -20 <file name> command you can read them. N stands for number in this command.
**syntax**
head -n (write number of lines you want to read) <file name>
```bash
head -5 filenew <img width="965" height="915" alt="image" src="https://github.com/user-attachments/assets/e0383adf-86dc-47ef-9056-b16914a386f9" />
``` 
* `tail -n` - use this command to read last lines of files. For example- you have a file containing 50 lines and you want to read only last 10 lines then, you can use this command `tail -10 <file name>`.
**syntax**
tail -n (write number of lines you want to read) <file name>
```bash
tail -5 my_file <img width="958" height="947" alt="image" src="https://github.com/user-attachments/assets/f97c5b9f-8380-42cb-ad9f-4adfc6e70aa4" />
```

* `apt` - Use this command to manage packages in linux. The benefit of using this command is that , when we install packages or applications from internet , instead of from computer then, it manages all work itself and install them. But when we use `dpkg -l` command, then it will not install packages from internet, it can not do this work. So, use `apt` for installing and `dpkg -l` for checking packages it they are installed or not. You can also use `apt` for checking packages if they are installed or not, but it will give you a warning due to unstable cli of apt.
**Syntax:**
`sudo apt install [package or application name]`  Use this for installing , instead of `dpkg`
`apt list --installed` (for checking all the installed packages)
`dpkg -l` (for checking all the installed packages with more readability and easyily)
`dpkg -l `|` grep [package or application name]`

dpkg shows only installed packages, from dbkg database, in better format

apt shows installed packages , from apt cache , a little bit complex machine language, but we can use grep to see single packages for checking.

apt list shows installed + uninstalled packages, from ubuntu repository, to see all the avalable packages that are uninstalled and installed packages.
apt cache pkgnames , to see only names of packages, from apt cache, scripting, grep to names search from them.

* `systemctl` - To check status, and do enable or disable a service.
**Usage Regarding Different Distros (other versions) of Linux:**
 #### For Ubuntu users :
**Syntax:**
`systemctl status [service name]` (ufw is a service of firewall by ubuntu for it's users)
To Start or Stop a service :
`systemctl stop [service name]` + sudo authentication. It requires `sudo` authentication, because ,if you want to stop or start a service ,it will bring some changes in your system so that's why it's authenticated when we want to stop or start a service.
#### For Redhat, Fedora , CentOs :


se this command to check status of a service, use `sudo` before systemctl when. you want to stop aur satrt a new service, because new service will derive new chnges in ypur sytem that why there is need to authenticate and sudo permisiion is needed, for redhat, fedora for example use systemctl firewalld.service and for ubuntu check systemctl status ufw, because servicces are different for different systems.



* `awk -f` - is command ka use file mein se kisi khaas column ko prinr krne ke liye hota hai , awk software ka naam hai jo mukhya files ko process karta hai aur -f ka matlab hai field separator yeh batata hai ki file comas se separte ki gai hai, mi=ukhya roop se csv (comma separetd values) files ko column dekhne ke liye use kiya jaata , print ka matlab hai screen par dikhao, aur dollar sign ka maening hai ki is clumn ko dikhao
usle baad csv file ka naam

* `cut -c` - ye command shabdon ko kaatne ke liye use hota hai, cut ek toll hai jo kaatat ha, -c yaani character aur uske baad no likhein yani numbers mein dekh kar batao, file ka naam likhein. yeh vertically kaat ta hai
* `sed` - is command ko ksis specific line ko katne ke liye use karein , sed -n '5p' file ka naam, ek aur cheez hai ismein, hum is sed 's/f/t/g' file name , command se chnage bhi kar sakte hain, aur bhi bahut kuch hai.
* `tr` - bhai is command se hum file ke content ko find , replace ya delete kar sakte hain, tr -d lowwr upp, matlba file ke saare text jo low hai upp kardo, iske baad tr punct, matlab jitne bhi punct hai unke remove kardo, aur tr -d digit , mataln digits no. remove kardo, tr '' '' <file, words replace karne ke liye,

* `truncate -s` - hum ye command ka use files ke size ko chota bada karne ke liye karte hain , truncate ka matlab hai aakar badalna ya resize karna , -s batata hai size uske baad size likhein aur file ka naam likhein , iska use developers ya sofware engineers testing ke liye karte hain ki unka app files ko download kar sakta hai ya nhi, choti badi files ke keraan yeh hota hai. aap khaali file ka size badha sakte hain , ghata sakte hain, par agar aapki file mein koi required data ya important informaton hai aur aap usse chota karne ki koshish karte hain uske bade size ke muqaable toh vo unte bite ki file banakar baaki ka data remove kar deta hai, isiliye is command ka sahi use mukhya roop se testing la hai, is command ko log files jinemin servrrs ki information rakhte hain, agar vo badi ho jaaye toh hum del karenge toh error aa sakta hai, toh hum vahan par i sec mein uska size zero kar dete hain, server logs file mein iska use isiliye hota hai, kyunki jaisa jiase server par users aate ahin toh unki saari information usmein store ho jaati hai jiske kaaran hum usse delete karne ke bajaye size chota kar dete hain

* `echo` - is command ko hum kisi cheez ko vertical line mein likhne ke liye use karte hain , echo abcde | fold -w2 , pehle echo likhein taaki print ho, fir line likhein, fir | use karein, fold -w2 , width bata dein.

* `sudo su` - ye command root user ko access banne ke liye use hota hai, sudo su likh kar password daalein apna jisse login hain aur kaam khatam karke exit ya ctrl + d dabayein, aapp root user access karenge toh kaam dhyaan se karna hoga galat deletion ya download dikkat kar sakta hai.

* `ssh user@hostname` -is command ka use kisi dusre remote server ko acces karne ke liye hota hai , ssh ka matlab hai secure shell, uske baad apna username daalo jisse app logged in ho, fir @ aur uske baad server ka ip ya domain name, jissse aap access karna chahte ho uska.. app direct windows, macos, terminal se, command chalakar ip add karke bina koi software download kiye, vm banyae , remote server access kar sakte ho, bas humein '-i' jiska matlab hota hai identity file iski key bannani padti hai, kyunki jab hum oracle , aws ya kisi bhi remote server ko access karte hain, toh humein key provide hoti hai, path isliye dena padta hai, taaki hum keh sakein ki ye key hai isse remote server ka taala khol do, server ke anadr hum apna saara kaam kar sakte hain, 24/7 access milta hai, jab hum laptop band kar dete hain, toh hum backend pe sabke liye live hi hote hain..

* `scp ` - is command ka use remote linux server par files ko copy karne ke  liye hota hai. scp file user@hostname:/tmp/ , scp ka matlab hai secure copy jo ssh ke zariye encrypted way se transfer hoti hai, tmp ka matlab hai file server ke tempo folder mein jaakar save hogi, agar server key based hai toh usmein key (-i my.pem) lagana padta hai, agar folder pura bhejna ho, toh -r recursive ka use karein scp ke baad.., key tab use hoti hai jab aap kisi server provider ke website par apna a/c banate ho aur fir server use karte ho, locally aap ne oracle vitua; box instal karke server use kar rahe ho, toh sirf password hi kaafi hota hai, kyunki vo aapke saamne hai, uske components touchab;le hai, jabki remote server us, uk mein data centre mein hai..

* `chmod` - is command ka use linux mein permisiions dene ke liye use kiya jaata hai, ls -ltr enter karke dekho, toh vahan par side mein `drw, rx, r ` jasa kuch aata hai, aur vo batatein hain ki kya permisiions hain, vahan par kuch names bhi likhein hote hain alag column mein, aur vahan se bhi pata chalta hai ki owner kon hai files aur folsers ka, u- user ,a-all, o-other, g-group ko access dene ke liye use kiya jaata hai.., u yyani user, group yaani team ke members, ek group ko di toh sab groups ko mil gayi, other yaani all over the world ko access de dena, r for read, w for write , for exetibales agar koi script ya software file hai toh usse command ki tarh chala dena

upar wala method symbolic tha, ab hum numerical method karenge, 
numeric method mein stanadrad 4 , 2 , 1 , 0 use hota hai..
4 user ko describe kart hai , ye koi user ke numbers nhi hain, bas users chahe kitne hon bas un sabko 4 se describe kiya jaata hai, 2 hai group , aur 1 hai other , aur 0 yaani koi permision nhi kisi ko bhi, for example , agar aap groups , ya other party ko access dena chahate hain, toh aap krenge - chmod 755, 7 ka  matlab (read 4, write 2, execute 1), yaani user sab kuch kar sakta hai, dusre no. par groups aa gaye, 4 yaani read , aaur 1 yaani execute (4+1=5), aur aise hi third party ko bhi 5 yaani read and write ki permsion hai. 
ek hota hai -644 - ismein 6 yaani 4+2 (read , write) for user, 4 yaani read for groups as well as other members.

NOTE: aap permissions requirement ke hisaab se de sakte hain, upar batayi gayi example s 755 (for scripts, softwares etc.) and 644 (for documents, files etc.)industry mein mostly use hoti hain, isliye unke prority de gayi lekin aap permissions zarroorat ke hissab se set karte ho, ye 700 ho sakti hai 7 yaani  (4+2+1 , r + w + x) baaki groups aur others 0 hain yaani unko koi permission nhi hai, toh at the end ye sab aapke upar hai..

* `chown` - iscommand ka use ownership change karne ke liye hota hai , in case aapko kisi file ki ownership change karni ho, toh chown yaani chnage owner command use karenge: pehle sudo su apply karein for ubuntu, password daalein aur ls -ltr ya ls -l aur file name likhkar pehle permission aur file name ache se check kar lein, uske baad chown name aur file ka name daalein aur enter karein.
* note : chmod chalane ke liye hamesha root user (sudo) ki zaroorat nahi hoti. Agar aap apni khud ki banayi hui file ki permission badal rahe hain, toh aap normal user se bhi chmod chala sakte hain.Lekin agar aap kisi system file ya dusre user ki file ki permission badal rahe hain, ya fir file ka owner badal rahe hain (chown / chgrp), toh Root Access (sudo) compulsory hai.

* `chgrp` -is command ka use group owner change karne ke liye hota hai, pehle sudo su karke root user se login karein, password daalkar, kyunki aise chnages karne ke liye root access chahiye hota hai, chgrp karke naam likh dein jaise ksis dusre ka ya fir apna logges in naam, file name likhein enter karein..
akeli ek file ki permissions aur syatus dekhne ke liye ls -l file namr likhein..

* `free` -is command ka use server ki memeory check karne kiye hota hai, kyunki memory limit hoti hai, free command chalyenge toh vahan par memeory aur swap information aa jayegi, kitni used hai, kitni bachi hai, aur baaki informatuion.. tips- free dabane par information dikh jayegi saari lekin kuch readable nhi hogi, readable banane ke liye free -h likhein aur total paane ke liye, free -th dabayein.. swap memory hoti hai, jab humari main ram khatm hone waali hoti hai bhar jaati hai haeavy tasks se, yoh linux ssd, hardisk se nakli ram banata hai taaki kaam kharaba na ho aur system crash na ho, isse kaam toh chal jaata hai , par slow chalta hai kyunki ssd se aane mein ram ko time lagta hai.

* `top` -is command ka use %memeory usages, cpu information aur bhi bahut saari information dekhne ke liye use hota hai,%cpu mein kitni cpu use ho rahi hai aata hai, aur aage ..id (ex- 97.5) ayega jo total bachi hui cpu% hai , aao 100 mein se usse minus karke used cpu nikal sakte hain, mib mem ye batata hai ki server ke paas kitni memory khali bacji hai aur kitni used hai, total kitni hai, mib swap se swap memory ka pata chla jayega, agar zero hai aapka toh matlab abhi kuch use nhi hua swap bankar ssd mein se..
Pehli Row (PID ...):Yeh process aapke total CPU ka ....(%CPU) consume kar raha hai.Aur aapki total RAM ka ...(%MEM) gher kar baitha hai.Doosri Row (PID ...):Yeh process CPU ka ...aur RAM ka ... use kar raha hai, q dabayein bahar aane ke  liye..

* `du` -is command ka use disk utilization yaani disk usage chack karne ke liye kiya hai, ki konnsi file, folder kitni disk usage kar rahi hai, kitna usage hai, du -h use karke disk usage numbers ko human readable bana sakte hain, h ka matlab hota ha human, aap h ko baaki sab isi hi commands ke saath use kar sakte hain..
--max-depth=1: Is flag ko lagane se terminal har folder ke andar ghus kar lambi list nahi banata, balki sirf main (top-level) folders ki total size ka clean summary dikhata hai.--exclude={snap,desktop,config}: Agar aap disk check karte waqt kuch system ya configuration folders (jaise snap, desktop, config) ko output se hatana chahte hain, toh is filter ka use karein.Syntax Example: du -h --max-depth=1 --exclude={snap,desktop,config}

* `df` -is command ka use disk space ke saath saath kuch alag information jaise , kitni used hai, avail kitni hai, use% etc.. df -h use kar sakte hain for better reading in (gb,mb,k)
Filesystem: Yeh batata hai ki disk ka kaun sa hissa hai. cloud server par aapko /dev/sda1 ya /dev/nvme0n1p1 jaisa naam sabse upar dikhega (yahi aapki main hard disk hoti hai).
size hota hai
used kitni hai
avail kitni hai
use % kitna hai
mounted on hota hai, linux mein folders ko kahin na kahin jidne ko mounting kehte hain, ismein root / directory hoti hai, jismein sab kuch bhara hota hai jo bhi sofware, command s etc..
ek tmpfs filesystem hota hai jismein saara kachra jaata hai, usmein asli / root hard disk ka kuch nhi hota usmein temporary cheezein hi jaati hain..

system info -linux mein system info aapke system ka identity card ya info card hota hai, heakth card, jo batata hai ki os kaisa, appka system kis hardware par chal raha hai etc. ye hardware details, cpu, ram , ssd, architecture jaise Batata hai ki system 64-bit (x86_64) hai ya ARM (aarch64).
software and os details, os distribution and releases, kernel hostname, ruuning and performance state, uptime , load average/cpu average , running time
* `hostname` -to check hostname of your linux server, menas the name of your vm (virtual machine), and it also sees only our terminal.
* `lscpu` -is command ka use cpu/core/thread info check karne ke liye use hoti hai.
* `arch` -is command ka use system ka archotecture check karne ke liye kiya jaata hai.
* `lsblk` - yaani list block is command ka use storage devices, disk partition, ki list dekhne ke liye kiya jaata hai.
* `uname -a` -is command ks use os ke mame ko jaan ne ke liye hota hai linux mein , ki hum kis naam ke os ka use kar rahe hain, hostname se pata chal jaata hai ki konsa os hai, par hostname hum chnage bhi kar sakte hain, toh thoda detail mein jaane ke liye hum uname -a ka use kar sakte hain, iske ilava hum cat /etc/os-release karke bhi info le sakte hain, farq itna hai ki ye humare os ditribution ki details deta hai, aur uname -a humare kernel ki
Linux mein /etc folder wo jagah hai jahan system ki saari configuration files aur metadata hota hai. /etc/os-release file mein OS ki identity key-value pairs mein save hoti hai.


PROCESS -linux meinprocess ka matlab hai koi chalta hua program, jab aap koi program ya command chlate ho toh process us code ko harddisk se uthakar ram mein load karta hai aur cpu ko deta hai isse hi process kehte hain, program- hard disk par rakhi hhui koi file ya code, ye tabb takk cpu par nhi jaata jab takk usse execute na kiya jaaye 
Process (Active): Jab aap us program ko open ya run karte ho, toh woh RAM mein load hokar Process ban jata hai. Ek hi program ke multiple processes bhi ho sakte hain (jaise Firefox ke 5 alag-alag tabs kholne par 5 processes ban sakte hain). ismein pid, ppid, s, owner, resouce allocatio, states check hoti hain, jaise running r , slleping s/d , zombie z , stopped , pid yaani processs id har process ko linux process id eta hai 2233, parent process id, yaani har processs ko ksis dusre process ne stsrt kiya hota hota hai , usse ppid kehate hain, owner ye batana hai ki process kis user scoount ki perm se chal raha hai
Resource Allocation: Process ko chalne ke liye RAM memory aur CPU cycles allocate hote hain.

tra Flags (Symbols):
+: Process foreground mein chal raha hai (aapke active terminal session par).

<: High priority process.

N: Low priority process.

* `ps -ef` -  1. ps -ef — Quick PID Lookup Aur Scripts Ke LiyeKaam: System ke saare processes ki ek static (ruki hui) snapshot list deta hai.Kab Use Karein: Jab aapko kisi specific app ka PID (Process ID) ya PPID (Parent Process ID) dhoondhna ho.Best Combination: Pipe grep ke sath test karna.Example: ps -ef | grep nginx (dekhne ke liye ki Nginx server chal raha hai ya nahi).
* 2. ps aux — Memory, CPU % Aur Process States Dekhne Ke LiyeKaam: Yeh bhi static list deta hai, lekin isme CPU%, MEM%, aur STAT (Process State: R, S, Z, T) jaisi detailed information hoti hai.Kab Use Karein: Jab check karna ho ki kaunsa process kitni RAM/CPU kha raha hai ya process Zombie (Z) state mein toh nahi hai.Example: ps aux | grep python3.
3.  top — Basic Live Monitoring (Har Server Par Available)Kaam: System resources (CPU, RAM, Load Average) aur processes ki real-time / live summary dikhata hai.Kab Use Karein: Jab aap kisi remote server par ho jahan koi extra tool install karne ki permission nahi hai.Khas Baat: Har Linux distribution mein pehle se inbuilt aata hai
4. htop — Best Interactive Task Manager (Daily Use)Kaam: Visual, colorful, aur interactive live monitoring tool.Kab Use Karein: Daily system monitoring, individual CPU cores ki health dekhne, aur frozen apps ko bina PID type kiye directly terminate karne ke liye.Khas Baat: Isme shortcuts hain — F3 (Search), F5 (Tree View), F9 (Kill).

* `pgrep` -is command ka use pid yaani sirf process id pata karne ke liye kiya jaata hai, yeh tabb takk apko pid nhi dikhayegi jabb takk vo proces ram mein run nhi hota . pgrep -l <name> likhne se pid ke saath process name bhi aa jaata hai, kyunki kai baar ek naam se dusre process bhi hote hai, ye keval 'active running' process id hi dikhata hai, ye background services jaise cron (automation tool in linux), sshd (remote server ke liye),systemd (लिनक्स का मेन मैनेजर जो सबसे पहले चलता है)networkd / NetworkManager (इंटरनेट और वाईफाई संभालने वाला)2. यूज़र ऐप्स और सॉफ्टवेयर (User Application) यूज़र ऐप्स और सॉफ्टवेयर (User Applications)कोई भी सॉफ्टवेयर जो आपने खुद स्क्रीन पर खोल रखा है।chrome या firefox (ब्राउज़र)vlc (मीडिया प्लेयर)code (VS Code एडिटर)
3. एक्टिव प्रोग्रामिंग स्क्रिप्ट्स (Running Scripts)अगर आप कोई कोड रन कर रहे हैं और वो जब तक चल रहा है।python3 (जब कोई पाइथन स्क्रिप्ट रन हो रही हो)bash या sh (टर्मिनल का अपना प्रोसेस)node (जावास्क्रिप्ट का बैकग्राउंड प्रोसेस)❌ pgrep किन चीज़ों का PID कभी नहीं दिखा सकता?बंद पड़े ऐप्स (Closed Apps): जो आपके कंप्यूटर में इंस्टॉल तो हैं (जैसे VLC), लेकिन अभी आपने उन्हें ओपन नहीं किया है।फाइलें और फोल्डर (Files/Folders): आपकी कोई मूवी, गाना या PDF फाइल (movie.mp4 या notes.txt) कोई प्रोसेस नहीं होती, इसलिए इनका PID नहीं होता।कन्फिगरेशन टूल्स (जैसे ufw): जैसा हमने पहले बात की, जो टूल्स सिर्फ सेटिंग बदलकर तुरंत बंद हो जाते हैं और बैकग्राउंड में लगातार नहीं चलते, उनका PID यह नहीं दिखा सकता।
  
* `kill`  2. pgrep कमांड (जासूस कमांड)यह कमांड रैम (RAM) के अंदर झाँक कर देखती है कि कौन सा प्रोग्राम इस समय एक्टिव यानी रनिंग कंडीशन में है।नियम: इस कमांड को एक बार में सिर्फ एक ही शब्द (पैटर्न) खोजने के लिए दिया जा सकता है। अगर आप स्पेस देकर दो शब्द लिखेंगे (जैसे: pgrep google chrome), तो एरर आ जाएगा।शर्त: यह बंद पड़े ऐप्स या नॉर्मल फाइलों (जैसे इमेज, वीडियो या पीडीएफ) की आईडी नहीं दिखा सकता।उपयोगी फ्लैग (-l): कमांड के साथ स्मॉल एल (-l) लगाने से केवल नंबर नहीं, बल्कि प्रोसेस का नाम भी लिस्ट के रूप में साफ़-साफ़ दिखाई देता है।3. प्रोग्राम को बंद करना: kill बनाम systemctlअक्सर लोग इन दोनों में कन्फ्यूज हो जाते हैं, लेकिन दोनों का काम बिल्कुल अलग है:सिस्टमctl (systemctl stop)यह केवल उन बैकग्राउंड सर्विसेस (जैसे Nginx सर्वर, SSH या फ़ायरवॉल) को रोकने के लिए है जो सिस्टम के साथ रजिस्टर होती हैं। यह नॉर्मल ऐप्स (जैसे Chrome या आपकी Python स्क्रिप्ट) को बंद नहीं कर सकता।किल कमांड (kill)यह सिस्टम में चल रहे किसी भी छोटे-बड़े प्रोसेस को उसकी PID नंबर के जरिए अस्थायी रूप से (Temporarily) बंद कर देता है। यह प्रोग्राम को कंप्यूटर से डिलीट नहीं करता, सिर्फ रैम से हटा देता है।इसके दो मुख्य तरीके हैं:केवल kill [PID]: यह सबसे सुरक्षित और समझदार तरीका है। यह प्रोग्राम को तमीज से अपनी फाइलें सेव करके बंद होने का सिग्नल देता है। हमेशा पहले इसी का इस्तेमाल करना चाहिए।kill -9 [PID]: यह ज़बरदस्ती बंद करने का तरीका है। जब कोई प्रोग्राम या स्क्रिप्ट बुरी तरह हैंग (Freeze) हो जाए और बात न सुने, तब इसका इस्तेमाल आखिरी रास्ते के रूप में किया जाता है।नाम से बंद करना (pkill)अगर आपको किसी प्रोसेस का PID नंबर नहीं पता और आप सीधे नाम से उसे बंद करना चाहते हैं, तो kill की जगह pkill कमांड का इस्तेमाल किया जाता है (जैसे: pkill chrome)।भाई, यह ड्राफ्ट एकदम तैयार है! क्या इसमें Nginx, Java या Chrome का कोई और उदाहरण जोड़ना है, या तुम इसे अब इंग्लिश में ट्रांसलेट करने की तैयारी करना चाहते हो? मुझे बताओ भाई!
pkill -9 bhi kar sakte hain, jab name se toh band karna hi ho, par jab forcefully ban karna ho atbb jaise kill ke saath kiya tha, sirf pause karna ho toh kill -stop pid, aur cont ya resume karna ho toh, kill -cont pid. pkill ya kill command se tempo cheez sirf pc ke on rehne takk hi off hoti hai, dubara on karne par automatic backend mein chalu ho jayegi. ye cheez sirf services par laagu hoti hai, jaise nginx, java etc.

**JOBS:**
terminal mein hum jo bhi command ya program chalate hain, usi ko hum jobs kehte hain, jab aap ek taraf gaana vagaira download kar rahe hote hain aur dusri taraf coding karni hoti hai tab jobs play mein aati hain
* fg foreground- jab aap koi command chalate hain aur terminal ki screen block ho jaati hai, aap agli command tabb takk nhi chala sakte, jab takk vo kaam pura nhi ho jaata.
* bg backgroung- isme aap apne ek kaam ya job ko background mein bhej dete ho, taaki vo background mein complete ho jaye, aur aapka terminal bhi free rahe jis par aap apna dusra kaam kar sakte ho, vo bacground wala kaam kahtam ho jayega.

**commands** 
-jobs - is command ka use background mein chal rahi saari jobs aur paused jobs ko dikhati hai, jo bg mein active hoti hain `jobs`
-ctrl + z - iska use kisi shuru kiye kaam ko pause karne ke liye hota hai, bg mein kaam pause ho jaata.
-bg -is command ka use bg mein kisi kaam ko chlau karne ke liye kiya jaata hai, taaki terminal free rahe, aur bg mein vo kaam pura bhi ho jaaye, 
syntax bg <%job_id> same aise hi fg yaani foreground ka hi hai.
1- =current job ko darsaati hai, 1- ka matlab hai pichli job, 2 ka matlab hai current job, 2- ka matlab hai pichli job.
 * `nohup ./script >dev/null &` -is command ka use kisi script ya program ko bg mein run karne ke liye liya jaata.


* `ip a` -is command ka use ip address check karne ke liye kiya jaata hai, ye aapke linux server ka ip batata hai, jo public hota hai.

* HOW TO CHECK IF A WEBSITE IS ACCESSIBLE OR NOT
* 
* curl -I https://google.com command ka use hota hai, http status check karne ke liye, ki website sahi work kar rahi hai ya nhi, agar kar rahi hai toh http/2 301/302 ayega.. agar 500/404 aata hai toh connection timeout ho jata hai , matlab gadbad hai koi toh.
* ping -c 4 google.com -is command ka use ye dekhne ke liye hota hai ki server jinda hai ya nhi, ye packets bhejta hai chote chote, -c 4 humnein isiliye use kiya ki bas 4 packets hi bhejo, aisa isliye kiya kyunki zyada likhne ya normal chlane se commnd, kaafi packets bhejkar check karti hai, agar 0 packets lost aaye aur ms mein answer aaye toh badhiya hai
* wget --spider https://google.com, ka use bina kuch download kiye sirf check karne ke liye kiya jaata hai, agar neeche remote file exists aa gaya toh matlab sab set hai, iska use basically automation running scripts ka quick check karne ke liye hota hai.

 नेटवर्किंग इन्फो में मुख्य रूप से 3 चीज़ें देखी जाती हैं:
1. IP Address (आईपी एड्रेस): आपके कंप्यूटर का डिजिटल घर का पता। (जैसे आपके घर का एड्रेस होता है, वैसे ही इंटरनेट पर कंप्यूटर का पता होता है)।
2. Network Interfaces (नेटवर्क इंटरफेस): आपके कंप्यूटर का वो हार्डवेयर (जैसे Wi-Fi कार्ड या Ethernet पोर्ट) जिसके ज़रिए इंटरनेट कंप्यूटर के अंदर आ रहा है।
3. Routing & Connectivity (कनेक्टिविटी): यह देखना कि आपका कंप्यूटर इंटरनेट के सर्वर से सही से बात कर पा रहा है या नहीं।

UNDERSTANDING NETWORKING INFORMATION IN LINUX:
Networking information allows us to check the system's IP address, active network cards (interfaces), and internet connectivity. This is essential for configuring servers and cloud environments.
MAIN NETWORKING COMMANDS:
• ip a — Displays all network interfaces and their assigned IP addresses. This is the modern standard command in Linux.
• hostname -I — A quick command to display only the local IP address of your system in a single line.
• curl ifconfig.me — Fetches and displays your Public IP Address (how your system is identified over the internet).
SYNTAX & EXAMPLES:
• To see full network details: ip a
• To see only your local IP: hostname -I


 1. Ports (पोर्ट्स) क्या होते हैं? (The Easiest Analogy)
इसे एक बहुत बड़े अपार्टमेंट (Apartment Building) के उदाहरण से समझो:
• मान लो तुम्हारा कंप्यूटर एक बहुत बड़ी बिल्डिंग है। उस बिल्डिंग का एक ही मुख्य पता होगा, जिसे हम IP Address कहते हैं (जैसे—बिल्डिंग नंबर 5)।
• अब उस बिल्डिंग के अंदर बहुत सारे अलग-अलग फ्लैट्स (कमरे) बने हुए हैं, जिनके अलग-अलग नंबर हैं। लिनक्स की दुनिया में इन्हीं फ्लैट नंबर्स को Ports (पोर्ट्स) कहा जाता है।
• काम कैसे होता है: जब इंटरनेट से कोई डेटा तुम्हारे कंप्यूटर (बिल्डिंग) तक पहुँचता है, तो उसे यह भी पता होना चाहिए कि उसे किस कमरे (पोर्ट) में जाना है। उदाहरण के लिए:
	• अगर कोई वेबसाइट खोल रहा है, तो डेटा सीधे कमरा नंबर 80 या 443 (Web Ports) में जाएगा।
	• अगर कोई कंप्यूटर को रिमोटली कंट्रोल (SSH) कर रहा है, तो डेटा सीधे कमरा नंबर 22 (SSH Port) में जाएगा।
• लिनक्स में नियम: एक पोर्ट पर एक समय में सिर्फ एक ही सॉफ्टवेयर "कान लगाकर सुन" (Listen) सकता है।
🔍 2. तुम्हारे स्क्रीनशॉट का पूरा पोस्टमॉर्टम (Step-by-Step):
आइए ऊपर से नीचे तक देखते हैं कि तुम्हारे टर्मिनल में क्या-क्या हुआ:
🚨 netstat पर एरर क्यों आया?
• जब तुमने netstat -tuln चलाया, तो Ubuntu ने कहा: Command 'netstat' not found।
• वजह: आज के नए Ubuntu (लिनक्स) सिस्टम्स में netstat पहले से इंस्टॉल्ड नहीं आता क्योंकि यह पुराना हो चुका है। अगर तुम इसे चलाना चाहते हो, तो तुम्हें पहले sudo apt install net-tools कमांड चलानी होगी। लेकिन हमें इसकी ज़रूरत नहीं है क्योंकि हमारे पास नया और तेज़ टूल ss मौजूद है!
📊 ss -tuln का वो बड़ा टेबल क्या कह रहा है? (Heading by Heading)
जब तुमने ss -tuln चलाया, तो एक बहुत ही सुंदर टेबल खुला। इसकी हर एक हेडिंग का मतलब समझो:
• Netid (Network ID): यह बताता है कि डेटा भेजने का तरीका क्या है। udp का मतलब है तेज़ लेकिन बिना गारंटी वाला कनेक्शन (जैसे वीडियो कॉलिंग), और tcp का मतलब है 100% सुरक्षित और गारंटी वाला कनेक्शन (जैसे वेबसाइट खोलना)।
• State (अवस्था):
	• LISTEN: इसका मतलब तुम्हारा कंप्यूटर इस पोर्ट पर पूरी तरह जाग रहा है और बाहर से आने वाले सिग्नल्स का इंतज़ार कर रहा है (पोर्ट ओपन है)।
	• UNCONN (Unconnected): यह आमतौर पर UDP पोर्ट्स के लिए दिखता है, जिसका मतलब है कि पोर्ट एक्टिव तो है लेकिन किसी फिक्स कनेक्शन से बंधा हुआ नहीं है।
• Local Address:Port (असली खजाना 💎): यह दिखाता है कि तुम्हारे कंप्यूटर का कौन सा हिस्सा किस पोर्ट नंबर पर काम कर रहा है:
	• 127.0.0.54:53 और 127.0.0.53%lo:53: यहाँ अंत में जो :53 लिखा है, वह DNS (Domain Name System) का पोर्ट है। तुम्हारा कंप्यूटर इसी पोर्ट की मदद से वेबसाइट्स के नामों (जैसे google.com) को आईपी एड्रेस में बदलता है।
	• 127.0.0.1:631 और [::1]:631: यहाँ अंत में जो :631 लिखा है, वह CUPS (Common Unix Printing System) का पोर्ट है। तुम्हारा लिनक्स सिस्टम प्रिंटर से कनेक्ट करने के लिए इस पोर्ट को ओपन रखता है। (नोट: यहाँ [::1] का मतलब IPv6 एड्रेस होता है)।
🧐 लास्ट में ss -tuln | grep :22 खाली क्यों आया?
• जब तुमने पोर्ट 22 को छानने के लिए grep :22 चलाया, तो नीचे की लाइन बिल्कुल खाली (Blank) आ गई और कुछ भी प्रिंट नहीं हुआ।
• वजह: इसका मतलब यह है कि तुम्हारे इस Ubuntu सिस्टम में SSH सर्वर (openssh-server) चालू या इंस्टॉल नहीं है। पोर्ट 22 इस समय पूरी तरह बंद (Closed) है, इसीलिए लिनक्स ने कोई आउटपुट नहीं दिया। अगर तुम sudo apt install openssh-server चलाकर उसे एक्टिव कर दोगे, तो यहाँ तुरंत LISTEN लिखा हुआ आ जाएगा!
📝 इस पेज को अपनी गिटहब गाइड में शामिल करने के लिए परफेक्ट इंग्लिश ड्राफ्ट:
तुम अपनी फ़ाइल में इस पूरे लाइव एक्सपेरिमेंट को इस बेहतरीन फॉर्मेट में लिख सकते हो:
WHAT ARE PORTS IN NETWORKING?
• An IP Address identifies your computer on the network, but a Port is a specific communication endpoint (like a room number inside a big building) dedicated to a particular service or application.
• For example, web traffic travels through ports 80/443, while secure remote access (SSH) uses port 22.
TECHNICAL ANALYSIS OF THE PORT SCANNING EXPERIMENT:
(यहाँ आपकी यह शानदार लाइव स्क्रीनशॉट वाली इमेज आएगी)
• Netstat Deprecation: Running netstat throws a not found error because modern Linux distributions deprecate it by default in favor of the faster ss command.
• Understanding Active Ports: The ss -tuln output shows that the system currently has two active services running locally:
	• Port 53 (LISTEN/UNCONN): The DNS service responsible for domain name resolution.
	• Port 631 (LISTEN): The CUPS printing service running on the local loopback address (127.0.0.1).
• Verifying Closed Ports: Running ss -tuln \| grep :22 returns a blank output. This confirms that no SSH service is currently running, meaning Port 22 is completely closed on this server.

PRO-TIP FOR FILTERING PORTS:
You can break down the flags and use these commands individually to filter your network traffic based on your requirements:
• ss -t — Shows only the active TCP connections on your server.
• ss -u — Shows only the active UDP connections on your server.
• ss -tl — Displays only the TCP ports that are currently in LISTEN mode.
• ss -ul — Displays only the UDP ports that are currently active.



HOW TO CHECK IF A PORT IS OPEN ON OUR OWN SERVER:
To verify if a specific port is open and actively listening on your local server, you should check the internal socket statistics rather than scanning from the outside.
COMMANDS & SYNTAX:
• ss -tuln — This is the modern and fastest standard command to list all active TCP (-t) and UDP (-u) ports that are currently in Listening (-l) mode, displayed in Numerical (-n) format.
• Filtering a Specific Port: To check a single port (e.g., Port 22 for SSH), combine it with the grep command.
EXAMPLES:
• To see all open ports: ss -tuln
• To check if Port 22 is open: ss -tuln | grep :22
EXPECTED OUTPUT:
If the port is active, you will see a line containing LISTEN in the output. If the terminal returns blank, the port is closed.

* HOW TO CHECK IF A IP: PORT IS ACCESSIBLE OR NOT

* 1. nc (Netcat) कमांड (सबसे बेस्ट और आधुनिक तरीका)इसे लिनक्स का स्विस-आर्मी नाइफ कहा जाता है। यह बहुत तेज़ी से बताता है कि पोर्ट खुला है या बंद।सिंटैक्स: nc -zv <IP> <PORT>-z: इसका मतलब है सिर्फ स्कैन करो, कोई डेटा मत भेजो (Zero-I/O mode).-v: इसका मतलब है वर्बोस (Verbose), यानी साफ़-साफ़ लिख कर बताओ कि क्या हुआ।उदाहरण:bashnc -zv 8.8.8.8 53
Use code with caution.आउटपुट कैसे समझें:अगर Connection to 8.8.8.8 53 port [tcp/domain] succeeded! लिखा आता है, तो पोर्ट पूरी तरह चालू (Open) है।अगर Connection refused या Timed out आता है, तो पोर्ट बंद है या फ़ायरवॉल उसे रोक रहा है।2. telnet कमांड (सदाबहार और पुराना तरीका)यह हर डेवलपर का सबसे भरोसेमंद और पुराना टूल है।सिंटैक्स: telnet <IP> <PORT>उदाहरण:bashtelnet 8.8.8.8 53
Use code with caution.आउटपुट कैसे समझें:अगर स्क्रीन पर Connected to 8.8.8.8 लिखा आ जाता है, तो पोर्ट चालू है। (इससे बाहर निकलने के लिए कीबोर्ड पर Ctrl + ] दबाकर quit टाइप करना पड़ता है)।अगर Unable to connect आता है, तो पोर्ट बंद है।3. curl कमांड (केवल वेब पोर्ट्स जैसे 80 या 443 के लिए)अगर आप किसी IP का सिर्फ वेब पोर्ट (HTTP/HTTPS) चेक करना चाहते हैं, तो आप curl का भी इस्तेमाल कर सकते हैं।सिंटैक्स: curl -I http://<IP>:<PORT>उदाहरण:bashcurl -I http://142.250.183.46:80
Use code with caution.आउटपुट कैसे समझें: अगर आपको HTTP रिस्पॉन्स कोड (जैसे 200 OK) दिखता है, तो पोर्ट चालू है।

HOW TO TRACE ALL HUBS (HOPS) IN A NETWORK PATH TO REACH A WEBSITE:
When you access a website, your network packets pass through multiple intermediate routers and gateways (known as Hubs or Hops) before reaching the destination server. Tracking this path is crucial for debugging network latency and routing issues.
COMMANDS & SYNTAX:
• traceroute — This command maps the entire journey of your network packet, displaying the IP address of each router (hop) and the time taken (in milliseconds) to reach it.
	• SYNTAX: traceroute <website_name>
	• EXAMPLE: traceroute google.com
• mtr (My Traceroute) — A powerful, modern tool that combines ping and traceroute. It opens a live, real-time diagnostic screen to monitor packet loss and latency across all hubs.
	• SYNTAX: mtr <website_name>

 README के लिए एक सुंदर और वीआईपी समरी टेबल:
कमांड	यह क्या करती है?	कब इस्तेमाल करें?
sudo reboot	सिस्टम को तुरंत रीस्टार्ट करती है।	अपडेट्स लागू करने या टर्मिनल हैंग होने पर।
sudo shutdown now	सिस्टम को तुरंत पूरी तरह बंद करती है।	काम खत्म होने पर सर्वर ऑफ करने के लिए।
sudo shutdown +10	10 मिनट का टाइमर लगाकर बंद करती है।	जब कोई बैकग्राउंड टास्क खत्म होने का इंतज़ार करना हो।
sudo shutdown -c	लगे हुए शटडाउन टाइमर को कैंसिल करती है।	गलती से लगे टाइमर को रोकने के लिए।
📝 इस टॉपिक को अपनी गिटहब गाइड में शामिल करने के लिए परफेक्ट इंग्लिश ड्राफ्ट (बोल्ड **** के साथ):
तुम अपनी फ़ाइल में यह टेक्स्ट सीधे जोड़ सकते हो, यह बहुत ही प्रोफेशनल लगेगा:
SYSTEM CONTROL COMMANDS (REBOOT & SHUTDOWN):
These commands are used to safely restart or power off a Linux system. They are crucial when managing headless remote servers or cloud environments where no physical buttons or graphical menus are available.
COMMANDS & SYNTAX:
• sudo reboot — Instantly reboots the system safely.
• sudo shutdown now — Power off the system immediately without any delay.
• sudo shutdown +<minutes> — Schedules a system shutdown after the specified number of minutes.
• sudo shutdown -c — Cancels a previously scheduled shutdown.
EXAMPLES:
• To restart right now: sudo reboot
• To power off in 5 minutes: sudo shutdown +5

कमांड	यह क्या करती है?	कब इस्तेमाल करें?
sudo adduser <name>	होम फोल्डर और पासवर्ड के साथ नया यूज़र आसानी से बनाती है।	हमेशा इसी का इस्तेमाल करें—यह सबसे सुरक्षित और बेस्ट है।
sudo useradd -m <name>	केवल एक बुनियादी यूज़र अकाउंट बनाती है।	जब ऑटोमेशन स्क्रिप्ट्स के अंदर बिना किसी सवाल-जवाब के यूज़र बनाना हो।
sudo usermod -aG sudo <name>	साधारण यूज़र को Admin (Sudo privileges) की ताकत देती है।	जब किसी नए डेवलपर को सिस्टम में फुल एक्सेस देना हो।
sudo deluser <name>	किसी बने हुए यूज़र को सिस्टम से डिलीट करती है।	जब कोई कर्मचारी प्रोजेक्ट छोड़ कर चला जाए।
📝 इस नए टॉपिक को README गाइड में शामिल करने के लिए परफेक्ट इंग्लिश ड्राफ्ट:
तुम अपने प्रोसेस वाले सेक्शन में इस पॉइंट को बहुत ही शानदार तरीके से जोड़ सकते हो, क्लाइंट को तुम्हारी लिनक्स एडमिनिस्ट्रेशन की समझ देखकर बहुत खुशी होगी:
USER MANAGEMENT IN LINUX (USER CREATION):
Linux is a multi-user system, meaning multiple users can log in and interact with the system simultaneously. Managing users efficiently is critical for system security and access control.
COMMANDS & SYNTAX:
• sudo adduser <username> — The recommended interactive command to create a new user. It automatically sets up the home directory, prompts for a password, and configures user details.
	• EXAMPLE: sudo adduser harsh
• sudo usermod -aG sudo <username> — Adds the newly created user to the sudo group, granting them administrative (root) privileges.
• sudo deluser <username> — Safely removes a user account from the system when it is no longer required.




 THE LOW-LEVEL APPROACH: USING THE useradd COMMAND
While adduser is the recommended interactive script for beginners, Linux also provides a low-level, non-interactive binary command called useradd.
By default, running just useradd <username> is very raw—it will not create a password, nor will it create a home directory for the user. To make it functional, you must manually pass specific flags.
SYNTAX:
sudo useradd -m -s /bin/bash <username>
UNDERSTANDING THE FLAGS:
• -m (Create Home Directory): Forces the system to automatically generate a dedicated home folder for the user at /home/<username>.
• -s /bin/bash (Set Default Shell): Explicitly defines Bash as the default command shell for the new user, ensuring they get a proper terminal environment when they log in.
SETTING THE PASSWORD FOR useradd:
Since useradd does not prompt you for a password automatically, you must manually set it right after creating the user by running the passwd command:
• COMMAND: sudo passwd <username>
• EXAMPLE: sudo passwd harsh (The system will then securely prompt you to type and confirm the new password).
📊 DIRECT COMPARISON: adduser vs useradd
To keep it crystal clear for your readers or clients, here is how they stack up against each other:
Feature	adduser	useradd
Command Type	High-level interactive script.	Low-level raw binary command.
Home Directory (/home)	Automatically created without any flags.	Requires the -m flag to be created.
Password Prompt	Prompts you to set a password instantly.	Requires a separate sudo passwd command later.
Best Use Case	When creating users manually in the terminal.	Perfect for automated DevOps / Bash scripts.


 MODIFYING EXISTING USERS: THE usermod COMMAND
The usermod command in Linux is used to modify a user's account settings after it has been created. Whether you need to change a username, update a home directory, or lock an account, usermod handles it seamlessly.
SYNTAX & POWERFUL FLAGS:
• Granting Admin Privileges (-aG): Appends the user to a specific supplementary group without removing them from their current groups. This is primarily used to give a user sudo (administrative) access.
	• COMMAND: sudo usermod -aG sudo <username>
• Changing Login Name (-l): Changes the login name of the user from old to new.
	• COMMAND: sudo usermod -l <new_username> <old_username>
• Locking and Unlocking Accounts (-L / -U): Temporarily disables or re-enables a user account for security purposes.
	• To Lock: sudo usermod -L <username>
	• To Unlock: sudo usermod -U <username>


SCHEDULING ONE-TIME TASKS: THE at COMMAND
If you want to execute a script or command automatically at a particular date or time only once in the future, Linux provides a dedicated utility called the at command.
Unlike recurring cron jobs, once the at job runs at its scheduled time, it finishes and removes itself from the queue permanently.
HOW IT WORKS (THE INTERACTIVE PROMPT):
When you run the at command with a specified time, it opens a special interactive prompt (at>). You type the commands or scripts you want to run inside this prompt, and then safely save it.
SYNTAX:
at <TIME> <DATE>
STEPS TO SCHEDULE A JOB:
1. Enter the at command with your desired time (e.g., at 11:30 PM).
2. The terminal will switch to an at> prompt. Type the full path of your script or command:
	• sh /home/harsh/secretkey/python/folder/script.sh
3. Press ENTER, and then press CTRL + D on your keyboard to save and exit. The system will confirm by printing a message like job 1 at Thu Oct 15 23:30:00 2026.
🎨 FLEXIBLE TIME FORMATS EXAMPLES:
The at command is highly intelligent and understands natural English time formats. Here are the most practical examples you can use:
• By Specific Time Today: at 23:30 or at 11:30 PM (Runs at exactly 11:30 PM today).
• By Specific Date: at 2:00 PM 10/15/2026 or at 14:00 15.10.2026 (Runs on October 15th).
• Using Relative Time: at now + 10 minutes or at now + 2 hours (Perfect for quick testing or delaying a script).
• Using Special Keywords: at midnight or at noon tomorrow (Extremely simple and clean).
📊 MANAGING THE SCHEDULED JOBS QUEUE:
Once a job is scheduled, you can check its status or delete it using these supplementary commands:
• atq (At Queue): Lists all the currently pending scheduled jobs along with their unique Job IDs.
• atrm <Job_ID> (At Remove): Deletes a scheduled job from the queue if you change your mind.
	• EXAMPLE: sudo atrm 1 (Deletes Job ID 1).

 IMPORTANT NOTE FOR RUNNING at JOBS:
For your scheduled at jobs to execute successfully, the background automation service (known as the atd daemon) must be active on your system. If your jobs are scheduled but not running, use these commands:
• To check the service status: sudo systemctl status atd
• To start the service (if stopped): sudo systemctl start atd
• To enable it permanently on boot: sudo systemctl enable atd

TROUBLESHOOTING: AVOIDING THE "GARBLED TIME" ERROR
• The Issue: If you type seconds while defining the time (e.g., at 07:08:00), Linux will throw a syntax error. Last token seen: : Garbled time error.
• The Reason: The at command only accepts time in HH:MM (Hours and Minutes) format. It does not recognize seconds.
• The Fix: Always omit the seconds. Use at 07:08 or at 07:08 AM instead of adding :00 at the end.


UNDERSTANDING OUTPUT REDIRECTION (> AND >>):
In Linux, you can redirect the output of any command into a physical file instead of printing it on the terminal screen.
1. THE OVERWRITE OPERATOR (>)
The single greater-than sign > redirects the output to a file. If the file already contains text, it will completely overwrite (delete) the old content and replace it with the new output.
• EXAMPLE: hostname > filess
2. THE APPEND OPERATOR (>>)
The double greater-than sign >> appends the new output to the end of the file without deleting its existing content.
• EXAMPLE: pwd >> filess
⚠️ CRITICAL NOTE FOR ENVIRONMENT VARIABLES:
You cannot redirect an environment variable directly by typing its name (e.g., USER > filess will fail with a command not found error). Variables are not standalone commands. To save a variable's data into a file, you must use the echo command along with the dollar sign ($):
• CORRECT WAY: echo $USER >> filess

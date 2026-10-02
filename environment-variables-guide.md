# Comprehensive Guide to Environment Variables & Package Management in Ubuntu

## Introduction to Environment Variables (ENVs)

Environment variables are those variables which carry information about our system executables packed in variables, basically it's like a **Diary** in which all the information about our system executables is written, whenever we execute a command or perform an operation, our system checks if the executed command is saved or not, **if it is written** in the variables, **the system** finds it out and give you the output, **otherwise it will throw a command error or simply fail to execute the command**.

* `printenv` -This command is used to **print all the environment variables** present in your system. It displays all the system information that is currently stored in variables.

**SYNTAX:**

* `printenv`

```bash
printenv
```
**FOR SEARCHING ONLY A SPECIFIC VARIABLE INFORMATION:**

**SYNTAX:**

* `printenv <VARIABLE_NAME>`

**EXAMPLE:**

* `printenv USERNAME`

```bash
printenv USERNAME
```

**EXPECTED OUTPUTS:**

* **OUTPUT of the `printenv` command**:

<img width="400" alt="image" src="https://github.com/user-attachments/assets/24cd1530-72a6-4696-9546-ab4b4a7fffbd" />

* **OUTPUT of the `printenv USERNAME` command**:

<img width="400" alt="image" src="https://github.com/user-attachments/assets/7de30470-d202-4861-93c5-8ffad1fc84d8" />

---

**USE THE FOLLOWING COMMANDS TO CHECK EXECUTABLE PATHS AND THEIR LOCATIONS:**

* `which` -For printing the path of any command.

**SYNTAX:** 

* `which <command name or software or application name>`

**EXAMPLE:**

* `which ls`

```bash
which ls
```

**EXPECTED OUTPUT:** (If the executable exists)

<img width="400" alt="image" src="https://github.com/user-attachments/assets/092d94f4-326d-41e9-9110-b5de3151289e" />

* If the executable does not exist (Expected Error) :

<img width="400" alt="image" src="https://github.com/user-attachments/assets/d9252147-0343-4dc5-835c-d943d62084b8" />

* The above error occurred, because the `java` is not installed on the system.

**NOTE:**

* Sometimes, other errors can occur due to a wrong executable name, incorrect execution, wrong syntax, or when older versions of applications and software are replaced with new ones.

---

* `whereis` -This command is more helpful than `which`, because it shows you some additional information along with **its** path like, **its** manual guide path, **its** service path etc.
 
**SYNTAX:**

* `whereis <command name or software or application name>`

**EXAMPLE:**

* `whereis python3`

```bash
whereis python3
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/9967f0bb-c36c-497d-86fb-452624ec4e7d" />

**RECOMMENDED:** 

* `whereis` -For **getting** all information about executables.

---

**FOR INSTALLING UNINSTALLED APPLICATIONS/SOFTWARE OR COMMANDS:**

* `sudo apt` -Use this command to install applications, commands or **software on your system from the terminal**. `sudo` is used before apt, because installing or changing something in the system, **ROOT** access is required. You have to **enter your password** for the account you are logged into.

**SYNTAX:**

* `sudo apt install <Application, Software or command name>`

**EXAMPLE:**

* `sudo apt install python3`

```bash
sudo apt install python3
```

**NOTE:** 

* When **you** install an **application**, software or any command using `apt` command, then **you** do not need to add their paths manually in our system, they are automatically created, **when** we install them. You can check by **using** `which` or `whereis` command, **to verify if the path was successfully created**. 

---

**FOR CREATING A TEMPORARY VARIABLE USING THE EXPORT COMMAND:**

**SYNTAX:**

* `export VARIABLE_NAME="value"`

**EXAMPLE:**

* `export MY_VAR="HARSH"`

**HOW TO CHECK OR PRINT IF THE VARIABLE HAS BEEN CREATED OR NOT:**

* `echo` command is used for **printing** something on the screen.

**SYNTAX:**

* `echo $<VARIABLE_NAME>`

**EXAMPLE:**

* `echo $MY_VAR="HARSH"`

```bash
echo $MY_VAR
```

**NOTE:**

* This command is used to make a variable for **temporary** work. It is not permanently saved in the system, **when you shutdown** your computer, it will be removed automatically.

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/94c4af57-2725-4c15-9a2f-af4e72f36b62" />

---

**FOR CREATING PERMANENT ENV VARIABLE (USING NANO FILE EDITOR):**

**Use Following Command This Way For** **Permanent creation:** 

* `export VARIABLE_NAME="value"`

**STEPS:**

**1**. First check the **presence of `.bashrc` file** by entering `s -la`, that is used to **view hidden files**. You can also use `ls -la <file_name>`, directly to see it.

**SYNTAX:**
* `ls -la` (To see **all hidden files and folders**.)

* `ls -la` <file_name> (To see **only a specific file**.)

**EXAMPLE:**
* `ls -la` (To see **all hidden files**.)

* `ls -la .bashrc` (To check only **`.bashrc` file**.)

```bash
ls -la
ls -la .bashrc
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/5b69d88b-9f71-417b-9ccb-f69a6dc31570" />

<img width="400" alt="image" src="https://github.com/user-attachments/assets/13d63297-dbff-42b9-b2c0-64b7723ef5ab" />

---
 
**2**. Then, **open the `.bashrc` file** using the nano file editor. 

**SYNTAX:**
* `nano` <file_name>
* `nano ~/.bashrc` (To **open `.bashrc` file**.)

**EXAMPLE:**
* `nano ~/.bashrc` (To **open `.bashrc` file**.)

```bash
nano ~/.bashrc
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/d541a9df-7442-4229-a194-5e08dd0ee927" />

---

**3**. After opening `bashrc` in the nano editor, **scroll down to the very end** of the file. Type your variable directly there using the `export` command.

**SYNTAX:**
* `export VARIABLE_NAME="value"`

**EXAMPLE:**
* `export MY_VAR="HARSH"`

```bash
export MY_VAR="HARSH"
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/a0d5d8a1-17ca-459e-bed6-6b8d01b4e42a" />

---


**4**. After writing your variable and its value, press **CTRL + O to save** (Write Out) the file, press enter and then press **CTRL + X to exit** it.

**5**. When you return to the terminal and try to view the variable, you won't see it yet. This is because you need to run **source ~/.bashrc** to **implement the changes** on your system. Use `echo` command to print the variable on your terminal screen.

```bash
echo $MY_VAR
source ~/.bashrc
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/e3864acc-7608-428f-a861-4348ce2815aa" />

---

**CONGRATS!! YOU HAVE SUCCESSFULLY CREATED YOUR FIRST ENV VARIABLE!**

**NOTE:** 
* Never modify the **.bashrc file** without a valid reason. Accidental changes—**even a single character or dot**—can lead to a **system crash or terminal malfunction**.
* Always use the **dollar sign ($)** when printing or calling your variable with the **echo command** (e.g., echo $VARIABLE_NAME).
* Always use a **leading dot** (.) before the filename for **hidden files**, just as we do for the **.bashrc file**.

---

**FOR CREATING PERMANENT ENV VARIABLE (USING VI or VIM FILE EDITOR):**

**Use Following Command This Way For** **Permanent creation:** 

* `export VARIABLE_NAME="value"`

**STEPS:**

**1**. First check the **presence of the `.bashrc` file** by entering `ls -la`, that is used to **view hidden files**. You can also use `ls -la <file_name>`, directly to see it.

**SYNTAX:**
* `ls -la` (To see **all hidden files and folders**.)

* `ls -la` <file_name> (To see **only a specific file**.)

**EXAMPLE:**
* `ls -la` (To see **all hidden files**.)

* `ls -la .bashrc` (To check only **`.bashrc` file**.)

```bash
ls -la
ls -la .bashrc
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/5b69d88b-9f71-417b-9ccb-f69a6dc31570" />

<img width="400" alt="image" src="https://github.com/user-attachments/assets/13d63297-dbff-42b9-b2c0-64b7723ef5ab" />

**STEPS:**

**2**. Open the **`.bashrc` file** in **the vi/vim editor** by entering the command and scroll down to the end of the file.
* NOTE - Both vi and vim editors are **the same**, vim is just an updated version. You can use both for editing files.

**SYNTAX:**
* `vi <file_name>` or `vim <file_name>`
* `vi ~/.<file_name>` or `vim ~/.<file_name>` (To **open hidden files**.)

**EXAMPLE:**
* `vi ~/.bashrc` or `vim ~/.bashrc` (To **open `.bashrc` file**.) 

```bash
vi ~/.bashrc
vim ~/.bashrc
```

**EXPECTED OUTPUT:**

**vi editor:**

<img width="400" src="https://github.com/user-attachments/assets/34289394-9650-4d47-bc73-4bdfc2d68692" />

**vim editor:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/1b6fabaf-6199-4b6a-ab9e-56fd7aaa1db8" />

---

**3**. Unlike the nano editor, we cannot type directly upon opening a file in **vi or vim**. First, we must switch to **Insert Mode** by pressing the **`i` key** **(Make sure Caps Lock is OFF)**. Once pressed, you will see **`-- INSERT --`** appear at the bottom of the screen. 

**SHORTCUT KEY:**
 **`i`** (To switch to **Insert Mode** and enable typing)

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/d424a619-35bc-4048-9703-dedaa5e8daa0" />

---

**4**. Now, you can start writing **environment variable**, edit or write any file. Once you have finished writing, press **`ESC`** (ESCAPE), then type **`shift + :wq`** and press **`ENTER`** to **save and exit**.

**SYNTAX:**
* `export VARIABLE_NAME="value"`

**EXAMPLE:**
* `export MY_VAR="HARSH"`

```bash
export MY_VAR="HARSH"
```

**SHORTCUT KEYS:**
`ESC` (Escape)
`SHIFT + :` and then `wq` to save and exit.

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/f2af329d-6681-43e9-9516-92b22f8e4eae" />

---
**5**. When you return to the terminal and try to view the variable, you won't see it again this time also. This is because you need to run **source ~/.bashrc** to **implement the changes** on your system. Use `echo` command to print the variable on your terminal screen.

```bash
echo $MY_VAR
source ~/.bashrc
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/04d9d096-dced-4cac-9107-6de380f1364c" />

---

**NOTE:** 
* Never modify the **`.bashrc` file** without a valid reason. Accidental changes—**even a single character or dot**—can lead to a **system crash or terminal malfunction**.
* Always use the **dollar sign ($)** when printing or calling your variable with the **`echo` command** (e.g., `echo $VARIABLE_NAME`).
* Always use a **leading dot** (.) before the filename for **hidden files**, just as we do for the **`.bashrc` file**.
* Use **`DELETE`** button to delete something that you wrote wrong, because **`BACKSPACE KEY` (BKSP)** may not work as expected in case of **vi or vim editor** for deleting.

---

**COMMAND FOR UNSETTING YOUR ENV VARIABLE AND ITS PATH:**

Use the **`unset`** command to remove or delete an environment variable from your current session. 

**SYNTAX:**
`unset <Variable_name>`

**EXAMPLE:**
`unset MY_VAR`

```bash
unset MY_VAR
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/2903afbd-b96d-49c0-bec1-a40c47030b30" />

**NOTE:**
* The variable **MY_VAR** used in the screenshot above is the same environment variable created in the previous steps. Please **do not be confused by it**.
* The **`unset` command** only deletes the variable **temporarily** from the current session. If you want to remove it **permanently**, you must manually delete its export line from the **.bashrc or .zshrc file**.

**COMMON MISTAKES TO AVOID: THE unset PATH EMERGENCY:**

* **Never** execute the **`unset PATH`** command directly in your terminal sessions. If you do this, your system will instantly forget the locations of all basic commands (like **`ls`, `nano`, `clear`**), throwing a **command not found** error because **`PATH`** is the core environment variable holding all executable binary paths.

**How to Fix This Issue (Two Reliable Solutions):**

* **Solution 1 (The Fresh Session Method)**: Simply close your current frozen terminal window and **open a brand-new terminal window**. This will refresh your environment and instantly restore all default system executables.

* **Solution 2 (The Instant Reset Command)**: If you want to fix it inside the same terminal session, execute the following command to manually reload the default Linux system paths:

```bash
export PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```
---

**CREATING VARIABLE FOR VERSION CHANGING:**

* Different softwares can have **multiple versions** installed on the same system. If you want to switch or change the software version based on your **project** requirements, or when **adapting to a new version**, you can create a dedicated variable inside the **`.bashrc`** file to handle this smoothly.

**Use the following steps to configure it:**

**STEPS:**

**1**. First, **check the current version** of the software installed on your system using the following command: 

* We use the  **`java -version` command** to check the current active version of Java (JDK).

```bash
java -version
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/47ab2d43-05f1-411e-bf48-ef21d6fb8a5a" />


**EXAMPLES FOR SOME OTHER SOFTWARE:**

* `Python 3: python3 --version`
```bash
python3 --version
```
* `Node.js: node -v`
```bash
node -v
```
* `Git: git --version`
```bash
git --version
```
* `MySQL: mysql -V`
```bash
mysql -V
```

---

**FOR CHECKING ALL THE INSTALLED VERSIONS (JAVA/JDK):**

* We can use **`apt list --installed | grep jdk`** command to see all the installed versions of java on our system.

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/fbfc67c9-1e7a-46c3-8fb0-9a9692d03e47" />

**NOTE:**

* Different software applications use different flags like **`-v`, `-V`, or `--version`**. If you are unsure, you can always check the official documentation using the **`man <command_name>` or `<command_name>--help`** flags to find the correct version command.
* You can use the `apt list --installed | grep <software name>` command for other software as well by simply changing the name at the end. Note that the `apt` command by default shows a warning stating it does not have a stable CLI interface, making it less ideal for automation scripts. However, it is **100%** safe to run manually in the terminal.

**COMMAND TO HIDE THE WARNING:** 

If you want to hide that annoying CLI warning and get a clean output, you can redirect the error to `/dev/null` like this:

`apt list --installed 2>/dev/null | grep jdk` 

```bash
apt list --installed 2>/dev/null | grep jdk
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/61d44b8b-e13f-42b1-8d1a-d3b2ceeeca1e" />

---


**2**. Now, use the **`export` command** to configure the **`JAVA_HOME` variable** (this name is widely used as per industry standards) and assign the path of the specific Java version to it.

Use the following steps to configure it:

**FOR FINDING THE JAVA VERSION PATHS:**

* **`/usr/lib/jvm`** is the default directory where all installed versions of Java (JDK) are saved.
* You can access this directory by using the **`cd` command** (e.g., cd /usr/lib/jvm).
* Once inside the directory, use the **`ls` command** to list all the available Java version folders.

```bash
cd /usr/lib/jvm
```
```bash
ls
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/8bd0a120-1883-4aca-b7a0-8f921b512b61" />

**DEFINING THE JAVA_HOME VARIABLE:**

* Now, select the folder name of the Java version you want to use (for example, **`java-11-openjdk-amd64`**) and define your **`JAVA_HOME` variable** like this:

`export JAVA_HOME="/usr/lib/jvm/java-11-openjdk-amd64"`

```bash
export JAVA_HOME="/usr/lib/jvm/java-11-openjdk-amd64"
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ffeb438d-d962-4654-91bb-bedd4053be78" />

**VERIFYING THE VARIABLE:**

* You can check if the variable is successfully set in your current session by using the **`printenv` command**.

**SYNTAX:**

`printenv <VARIABLE_NAME>`

**EXAMPLE:**

`printenv JAVA_HOME`

```bash
printenv JAVA_HOME
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/9b29161c-6b1f-4f11-b28a-a1f4ab57b2cf" />

---

**3**. Now, even though the **`JAVA_HOME` variable** is set, the system still doesn't know where to find the Java executable binaries. To fix this, we must append the Java binary directory to the system's main **`PATH` variable**.

* We will implement this by using the following command (make sure there are no spaces):

`export PATH=$JAVA_HOME/bin:$PATH`

```bash
export PATH=$JAVA_HOME/bin:$PATH
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/db08798b-fe9d-4e57-827f-90c2ce47ede7" />


<img width="400" alt="image" src="https://github.com/user-attachments/assets/020757a9-adb1-46a5-9576-e281bdebde0e" />


* As you can see, before updating the path, the **`java -version` command** showed **Java 17** active on the system.
* Once the **`export PATH` command** was executed, checking the version again successfully confirmed the switch to **Java 11**.

---

**CONGRATS!! YOU HAVE SUCCESSFULLY CREATED A VERSION-SWITCHING ENVIRONMENT VARIABLE AND IMPLEMENTED IT!**

**NOTE:**

* All of this might seem difficult for you at first, but if you follow the steps and commands carefully and read all the notes, it becomes very simple.THANK YOU

**THANK YOU**

---

**DO WE NEED TO CREATE AN ENV VARIABLE OR DEFINE ITS PATH FOR INSTALLED SOFTWARE ?**

* It highly depends on how the software is installed. If we install it using the **`apt` command with root privileges (`sudo`)**, `apt` automatically handles all dependencies and background processes. It places the executable binaries directly into standard system folders (like **`/usr/bin`**) that are already part of the default `PATH`.
* You can verify if the location or path is automatically managed by using the **`whereis`** or **`which`** commands.
* On the other hand, if we install software manually using the **`dpkg` command**, we often need to manually **define an environment variable** and append its binary path to our system.
* Therefore, the **`apt` command** is highly recommended because it simplifies multiple tasks like installing, updating, upgrading, and removing software effortlessly.

**CONCLUSION & NOTE:**

* If software is installed using the **`apt` command**, there is **no need** to manually define any environment variables. However, if software is installed via the **`dpkg` command**, you must manually define its binary path to your system configuration.
* **Superuser privileges (`sudo`)** are required in both cases to perform these system-wide operations successfully.

---

**HOW TO OPEN A SOFTWARE IN THE TERMINAL ?**

* We can launch software directly from the terminal. To understand how this works, let's look at the two main types of software:
	**1**. **GUI (Graphical User Interface)**: Software that has a visual desktop interface that we can see and interact with (e.g., **`Google Chrome`, `VLC Media Player`**).
	**2**. **CLI (Command Line Interface)**: Software that operates entirely inside the terminal screen (e.g., **`Python3`**). In CLI applications, we only interact by typing commands and writing code, without any fancy desktop windows.

**LAUNCHING CLI vs GUI SOFTWARE (USING):**

* **For CLI Software**: Simply type its full name (like **`python3`**) as a command in the terminal to start coding. You can use the **`exit()`** function or command to safely close it.
* **For GUI Software**: You can also type their binary names (like **`google-chrome`**) in the terminal. However, the software will open in a separate desktop window, and your terminal will remain **frozen (blocked)**, meaning you cannot execute any new commands in that terminal window.

**USING CLI SOFTWARE (`python3`) IN TERMINAL:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/e54b4b71-8ab2-4ecd-af73-8edffc8dec51" />

```bash
python3
```

**PRO TIP TO PREVENT TERMINAL FREEZING:**

* To prevent your terminal from freezing, always use an **ampersand sign (`&`)** right after the GUI software name (e.g., **`google-chrome` `&`**). This forces the GUI application to **run as a background job**, leaving your terminal completely free for other tasks.

**USING GUI SOFTWARE (`firefox`) in TERMINAL WITH `&`:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/db17ad8d-84a0-4ae2-95c7-9c88dd4fece9" />

```bash
firefox &
```

**NOTE:**

* In the terminal screenshot above, running the **`firefox &`** command launches the Firefox application in the background. While the graphical interface (desktop window) opens separately and is not captured within the terminal screenshot, the browser is fully active.

**TECHNICAL ANALYSIS OF THE BACKGROUND JOB:**

* **The Ampersand Magic (`&`)**: Running **`firefox &`** instantly creates a background job. The system outputs **`[1] 39954`**, where **`1`** is the **Job ID** and **`39954`** is the **Process ID (PID)**. This prevents the terminal from freezing.
* **The `Ctrl + C` Behavior**: Pressing **`CTRL + C (^C)`** on the active terminal has no breaking effect on the application because the terminal thread is already free and the process is safely isolated in the background.
* **Graceful Exit**: Clicking the **'X' close button** on the Firefox window safely terminates the process. Linux immediately outputs **`[1]+ Done firefox`**, confirming that the background job has successfully finished and cleared from the memory.

**NOTE:**

*  You can open and close GUI software or applications even without using the ampersand **(`&`)** sign or **`CTRL + C`** (in some desktop use cases), and it is completely fine. However, when working on head-less remote servers like **AWS or Azure**, there are **no physical components or graphical interfaces** to interact with. In those real-world environments, the background job controls and termination commands discussed above become absolutely critical.


**DEFINING AND CREATING CUSTOM ENVIRONMENT VARIABLES:**

* Linux allows you to create your own custom paths and environment variables to store specific system configuration information based on your project requirements.

* Use the **`mkdir -p`** command to generate deeply nested directory structures (multiple folders inside folders) seamlessly at one time.

**TEMPORARY CREATION:**

* If you want to create a custom **temporary variable** for your current session, use the following command (make sure there are **no extra spaces** around the **`=`** sign):

**SYNTAX:**

`export VARIABLE_NAME="<YOUR CUSTOM PATH>"`

**EXAMPLE:**

`export MY_SECRET_FOLDER="path/to/you/secret/folder"`

```bash
export MY_SECRET_FOLDER="path/to/your/secret/folder"
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/32b1096a-c36f-4cb1-b7bf-5f516e923eab" />

**NOTE:**

* Creating a custom **environment** variable is highly recommended for long and deeply nested directory structures, as remembering complex absolute paths can be difficult.
* Always use the **`$` (dollar sign)** before the variable name to print its content.
* Since this creation method is **temporary**, the variable will be instantly removed once you close the terminal or restart your computer.

**FOR PERMANENT CREATION:**

* To make your custom variable permanent, we need to declare it inside the **`.bashrc`** configuration file, just like we configured the Java paths earlier.
* You can open and edit the **`.bashrc`** file using text editors like **`nano` or `vi`/`vim`**.
* In this guide, we will proceed using the **`nano` editor** as it is simple and beginner-friendly (though the **`vi`/`vim`** process has already been covered in detail above).

**STEPS:**

**1**. 1. First, create a folder using the **`mkdir`** command. If you want to create a deeply nested or deeper path structure, use the **`mkdir -p <parent_folder>/<child_folder>`** format. For a single standalone directory, simply use the **`mkdir <folder_name>`** command.


**Syntax:**

`mkdir -p foldername/foldername/foldername`

**EXAMPLE:**

`mkdir -p path/to/your/secret/folder`

```bash
mkdir -p path/to/your/secret/folder
```

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/14dd51c5-5970-4e5f-b22f-82ee657b6d4f" />

**NOTE:**

* As demonstrated in the screenshot, running the **`cd`** command right after allows you to successfully navigate or access+  into the newly created deep directory path without any errors.

**EXPECTED OUTPUT:**

**WRITING THE VARIABLE INSIDE THE `.bashrc` FILE:**

* Open your configuration file and go to the very bottom. Describe your custom environment variable using the **`export`** command as shown below:

```bash
export MY_SECRET_FOLDER="path/to/your/secret/folder"
```

<img width="400" alt="image" src="https://github.com/user-attachments/assets/66809fb6-4d75-49f9-aa3c-f178fc2558b6" />

**APPLYING CHANGES IMMEDIATELY:**

* We use the **`source ~/.bashrc`** command to instantly apply the new changes to our current terminal session without needing to log out or restart the system.


```bash
source ~/.bashrc
```
**NOTE:**

* This process is identical to how we reloaded the profile after configuring the **Java environment variables** earlier. The creation and implementation logic remain exactly the same, so do not get confused.


**HOW TO KEEP YOUR .bashrc FILE SAFE?**

* Whenever you add new variables or make changes to your .bashrc file, it is highly recommended to create a backup copy. This ensures you have a clean restore point if something goes wrong.

* You can execute the following command to duplicate your file safely:

```bash
cp ~/.bashrc ~/.bashrc.bak
```

**BREAKDOWN OF THE COMMAND:**

* cp — Stands for copy.
* ~/.bashrc — The original target file located inside your home (~) directory.
* ~/.bashrc.bak — The new backup file that will store a copy of your configuration.

**SYNTAX:**

`cp <real_file_name> <copied_file_name>`

**EXAMPLE:**

`cp ~/.bashrc ~/.bashrc.bak`

**EXPECTED OUTPUT: VERIFYING THE BACKUP**

**1**. **Executing the Command:**

* Execute the **`cp`** command in your terminal. It will run silently without throwing any output or errors, meaning the file duplication was successful.


<img width="400" alt="image" src="https://github.com/user-attachments/assets/3bc46893-bf70-4f2d-9dde-191bcbe5cfad" />


**2**. **Verifying the Copied Version of the .bashrc File:**

* To verify and ensure that your backup file **(`.bashrc.bak`)** contains the exact same configuration code, use the **`cat`** command to view its contents:

```bash
cat ~/.bashrc.bak
```

<img width="400" alt="image" src="https://github.com/user-attachments/assets/4b41b1aa-db48-41f2-a782-854e7ffec0b5" />

**CHECKING ITS PRESENCE:**

* Since any file starting with a dot **(`.`)** is treated as a **hidden file** in Linux, running a standard ls command will not display it.

* To verify the physical existence of your backup file, you must list hidden files or check it specifically using the long-listing **`ls -l`** command.

<img width="400" alt="image" src="https://github.com/user-attachments/assets/e7a15e6e-9375-4636-af6f-8d58c997da5c" />

**BREAKDOWN OF THE SCREENSHOT VERIFICATION:**

**1**. **Hidden File Behavior:** When you duplicate **`.bashrc`** to **`.bashrc.bak`**, the new backup file remains hidden. If you try to find it using a normal **`ls`** command, it will not appear in the terminal output.

**2**. **Using Long Listing (`ls -l`):** To view specific details and confirm the file is safely stored, execute the long-listing command followed by the precise file path:

```bash
ls -l ~/.bashrc.bak
```

As shown in the output, the system successfully displays the file permissions, size, and timestamp, proving the backup exists.

**NOTE:**

* When you use the **`cat ~/.bashrc.bak`** command to view a large configuration file, the terminal will quickly scroll down to the very end of the text. To read the entire file from the beginning, simply **scroll up** manually inside your terminal window.

**IF YOUR `.bashrc` FILE CORRUPTS, DO THIS:**

You can recover your system using **two reliable methods**. Here is the first method if you followed the safety rule and created a backup earlier:

**Method 1: Restoring from your existing Backup File**

* If you already have a safety backup, you can easily overwrite the corrupted configuration file using the copy command:

```bash
cp ~/.bashrc.bak ~/.bashrc
```

**BREAKDOWN OF THE COMMAND:**

* In this recovery scenario, we simply reverse the source and destination paths. We are copying our healthy backup file **(`~/.bashrc.bak`)** back over the corrupted original file **(`~/.bashrc`)** to replace it.


```bash
cp ~/.bashrc.bak ~/.bashrc
```

**Method 2: Reloading the System Configuration**

* After successfully restoring the file, you must reload the configuration or changes immediately to update your current terminal session:

```bash
source ~/.bashrc
```

**IF THERE IS NO BACKUP FILE (.bak), DO THIS:**

If you completely ruined your configuration and forgot to create a safety backup, do not panic. Linux stores a default, pristine template file hidden inside your system configuration folders. You can use it to completely **factory reset** your environment.

**1.** **Copying the Default System Template:**

* Execute the following command to overwrite your corrupted file with the original factory-fresh template from the **`/etc/skel/`** directory:

```bash
cp /etc/skel/.bashrc ~/.bashrc
```

**2**. **Applying the Changes Immediately:**

* After copying the default template, you must reload the configuration immediately to update your active terminal session without logging out:

```bash
source ~/.bashrc
```


## THANK YOU TO ALL ##










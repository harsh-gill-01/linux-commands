# Comprehensive Guide to Environment Variables & Package Management in Ubuntu

## Introduction to Environment Variables (ENVs)

Environment variables are those variables which carry information about our system executables packed in variables, basically it's like a **Diary** in which all the information about our system executables is written, whenever we execute a command or perform an operation, our system checks if the executed command is saved or not, **if it is written** in the variables, **the system** finds it out and give you the output, **otherwise it will throw a command error or simply fail to execute the command**.

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

* `echo` command is used for printing something on the screen.

**SYNTAX:**

* `echo $<variable name>`

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

---

**CREATING VARIABLE FOR VERSION CHANGING:**

* Different softwares can have **multiple versions** installed on the same system. If you want to switch or change the software version based on your **project** requirements, or when **adapting to a new version**, you can create a dedicated variable inside the **`.bashrc`** file to handle this smoothly.

**Use the following steps to configure it:**

**STEPS:**

**1**. First, **check the current version** of the software installed on your system using the software name like these:

* Python 3: python3 --version
* Java: java -version
* Node.js: node -v
* Git: git --version
* MySQL: mysql -V

**NOTE:** I showed -v, -V, --version for finding version of different softwares. This is because there are their own rules as per finding their version.

**2**. 
when you want to execute a software in your terminal, there can be two or more versions of it, check its version by writing -version before its name, and check which version is running, if waanna chnage version, make env, variaable as per using export or nano command, for requirements, execute it, describe path there save it , sourse for rapid implementaion for rapid work,ctrl, click x for come out  , if software or application has cli, no face or desktop , then type it in terminal, do your wwork, exit for coming out, if its gui which has its oen desktop website, then it type its name as well, but it will open in another window not in terminal, terminal will be locked in this case, exit the gui application or software, then terminal will be opened , use & , after name of software so that terminal , agar chat he ki termi khuli rahe aur soft chlta rahe, toh & bhi barte saath mein , hum apni tarf se kuch bhi path bana toh sakte hain par linux mein jab vo chalega toh error aa jayega kyunki apne jo khud se folder name diye hain vo exixst nhi karte, agar PATH mein bhi  karoge toh bhi, export mein bnhi, solution pehle mkdir -p se random path banadein fir varibale bana dein export ya nano karke kaam ke hi saab se, iske baad jab bhi aap karoge toh aaram se vo khul jayegam ye sab custom env se sambhav ha
version check karne ke liye , -v aur --v ka chakkar zyada nhi hai, java kjaise purane soft ke kaaran -v use hota hai, agar vers chec karn ha, pa pata na kaa likhe,toh man ya help command use kar sakat he ya -v air--v dono type kare


emv variables vo hote jinmein variable mein kuch information store ki hoti hai, ye humare system ki diary hoti hai, hum jo bhi kaam karte hain, system diary mein dekhta hai, agar usse vo mil jaata hai toh output mil jaata hai, agar vahan vo information nhi hai toh error aa jaata hai ya kuch nhi hota, inmein har ek information store nhi hoti jaise user name, permissions, home name, names , system ki information vagiara, jo computer ko chalane mein help karti hain vo hi sab cheezein hoti hain , agar koi file ya information humari kisi drive mein hai toh hum uska path variable banakar save zarooor kar sakte aur usse terminal mein open karke dekh bhi sakte hain, bas itna hai kihumein usse define karna padta hai export se for tempo and nanobashrc for permanent, kyunki computer mein pehle se sab kuch nhi hota, isiliye hum apni require ke hisab se batadete ya define karte hain ki is information ko bhi apni diary mein note karlo. simple .....///, ab aaap path banayegenge , system mein nayi cheezein add karenge toh delete bhi karni hongi taaki ram full na ho, toh hum unset command use karte hain, hum bas variable ka naam likh dete hain aur unset command daalte hi , vo innfo delete ya remove ho jaati hai syst se, kabhi home mein reh kar seddha unset path mat karna kyunki isse system apne saare path ko hi delete kar deta hai aur baad mein jab aaap kuch comm, chalaoge toh nhi chelga , agar aisa kabhi hota hai toh ye ....PATH.... command use karein isse aapke basic commands sab activate ho jayenge, par agar aapne alag se variables banaakr kuch add kiya hua tha toh vo ismein nhi ayega, aur haan agar aapne bashrc mein path delte kar diya tha toh vahan par hi theek karna hoga , taaki permanent save ho PATH, agar terminal se command chlayo thi, toh upar wali command chalyein theek ho jyayega , agar aap apne dusri soft, info, ya file, fold, ko bhi vaapis laana chat hain toh ya toh linux ka bacshrc backup file check karein, ya fir export PATH: likh kar aage apna path jodkar us ko vahan par rakh sakte hain dubara se, agar folder apni marzi se name dekar banane hain toh mkdir se pehle folder bana dein isse appka system fir se unhe save kar lega aur app chala paoge flutter, java etc, ko bash rc mein likhna hoga par agar aapki bashrc kharab ya corrupt ho jaaye tph aap isse aise karke jo real default bashrc hai usmein jaakar saara code copy karke dubara se basgrc mein daal sakte hain jisse bilkul fresh file dubara ready ho jyegi, aap real skel bashrc mein changes nhi laa sakte, par apni copy basgrc mein laa sakte hain, aur jo bhi path soft,info purane mein thi, is nayi mein dubara daal kar save kar lijiye, bashrc kabhi bhi export path ka bcakup nhi rakhta kyunki vo banaya hi tempo hota hai, toh backup aur permanent ke liye real bachrc mein likh dein saara path......./etc/skel/.bashrc ~/.bashrc  ,read karein, cat /etc/skel/.bashrc
bhai, version chnage karte waqt pehle ek variable baan lein jaise ..., aur usko path ke saath, jismein vo real change waala version hai saath jodein isse vo varoable mein save ho hua, iske baad ... karke usse daal dein, ab aapko pura path nhi likhna pada aapne bas varibale name likha aur uske baad ...path likhein aisa isliye kyunki version chnage ke waqt pehle path desribe hota hai. softeware ke naam ke saane hum var nhi kar sakte, vahan humein path se hi save karna padta hai, env variable soft ya version ke waqt kaise aur kahan banana hai :
agar software installed hai pehle se , apt command se installed kiya hua hai toh, seedha software ka naaam daal kar enter dabayein soft terminal mein khul jayega , humein paths unke banane padte hain jo amnully download kiye gaye hain jaise java,flutter, sdk,etc. aur jo package manager ke custom tools ya fir kuch secret information jaise database, api keys, etc. inke liye sabse pehle naya path banayein , which ya whereis command se check karkefir purana path jod dein, database aur api keys ke liye sirf normally variable banakar store karein, iske ilava softwares ke versions chnage karne ke liye pehle naya version path jodein aur baad mein purana taaki aapp naye version ko use kar sakein. jab hum software ko terminal mein khilte hain toh vahan par save karne ka koi tarika  nhi hota humare kaam ko isliye professinals pehle vs code ya nano chalakar usmein code likhte hain aur file banate hain aur baad mein usse run kar dete hain python mein aur output dekh lete hain file banakr rakhne se code ssd mein save ho jaata hai file mein ,software bas test ke liye aur output paane ke liye hota hai. 









# Comprehensive Guide to Environment Variables & Package Management in Ubuntu

## Introduction to Environment Variables (ENVs)

Environment variables are those variables which carry information about our system executables packed in variables, basically it's like a diary in which all the information about our system executables is written, whenever we execute a command or perform an operation, our system checks if the executed command is saved or not, if it will be there written in the variables, it will find it out and give you the output, otherwise a command error or simply no execution of the command will be thrown.

---

**USE THE FOLLOWING COMMANDS TO CHECK EXECUTABLES PATH AND THEIR LOCATION:**

* `which` - For printing the path of any command.

**SYNTAX:** 

`which <command name or software or application name>`

**EXAMPLE:**

`which ls`

```bash
which ls
```

**EXPECTED OUPUT:** (If executable will be there)

<img width="400" alt="image" src="https://github.com/user-attachments/assets/092d94f4-326d-41e9-9110-b5de3151289e" />

* If the executable will not there (Expected Error) :

<img width="400" alt="image" src="https://github.com/user-attachments/assets/d9252147-0343-4dc5-835c-d943d62084b8" />

* The above error occured, because the `java` is not installed there in the system.

**NOTE:**

Sometimes there can also be other errors due to, wrong executable, wrongly executed, wrong syntax, and sometimes due to replacement of old versions with new ones of many applications, and softwares.

---

* `whereis` - This command is more helpful than `which`, because this command shows you some other information along with it's path like, it's manual guide path, it's service path etc.
 
**SYNTAX:**

`whereis <command name or software or application name>`

**EXAMPLE:**

`whereis python3`

```bash
whereis python3
```

**EXPECTED OUPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/9967f0bb-c36c-497d-86fb-452624ec4e7d" />

**RECOMENDED:** 

`whereis` For geting every information about executables.

---

**FOR INSTALLING UNINSTALLED APPLICATIONS/SOFTWARES OR COMMANDS:**

`sudo apt` - Use this command to install applications, commands or softwares in your system from terminal. `sudo` is used before apt, because for installing something and to change something in system, *ROOT* access is required. You have to fill you password, to which you are login within your system.

**SYNTAX:**

`sudo apt install <Application, Software or command name>`

**EXAMPLE:**

`sudo apt install python3`

```bash
sudo apt install python3
```
**NOTE:** 

When you install an appliaction, software or any command using `apt` command, then we do not need to add their paths manually in our system, they are automatically created and we install them. You can check by usuing `which` or `whereis` command, if it's created or not.

---

**FOR CREATING TEMPORARY VARIABLE:**

**USING EXPORT COMMAND:**

**SYNTAX:**

`export VARIABLE_NAME="value"`

**EXAMPLE:**

`export MY_VAR="HARSH"

#HOW TO CHECK OR PRINT IF THE VARIABLE HAS CREATED OR NOT:

`echo command is used for printing something on the screen.`

**SYNTAX:**

`echo $<variable name>`

```bash
echo $MY_VAR
```

**NOTE:**

*This command is used to make a variable for temporaray work, it's not saved in the system, when you will shutdown your computer, it will be removed automatically.

**EXPECTED OUTPUT:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/94c4af57-2725-4c15-9a2f-af4e72f36b62" />

---

**FOR CREATING PERMANENT ENV VARIABLE:**

#Use Following Command This Way For Permanent creation 

`export VARIABLE_NAME="value"`

**STEPS:**

*Open any file editor `vim` or `nano`. We are using nano








use which command to see, at present the software you want to env, add inw hich path its running and whereis command to check the path, its suitables files and folders, its manula guide , all the paths.
use export path=path///// command for temporary env variable of your software
use nano ~/.bashrc, use nano~/.zsh in case of this sshell, write export path=path///// at the end of the file by scrolling down, press ctrl+o for save and enter press, ctrlx for come out,rapid implement for source~/.bashrc
its a keyvalue pair , menas its a in it all the onformation and settings are stored.there are also other things like user , home to see your user name information and home path, you can customize also, make your own variables to store information and path , due to this we can describe our own path, its the file or folder is very deep, we can make a env by export command , but it will be removed or chnaged after the system is shut down, use nano to edit permanenetly path , use unset command for unsetting the varibale custom
will be removed..
when you want to execute a software in your terminal, there can be two or more versions of it, check its version by writing -version before its name, and check which version is running, if waanna chnage version, make env, variaable as per using export or nano command, for requirements, execute it, describe path there save it , sourse for rapid implementaion for rapid work,ctrl, click x for come out  , if software or application has cli, no face or desktop , then type it in terminal, do your wwork, exit for coming out, if its gui which has its oen desktop website, then it type its name as well, but it will open in another window not in terminal, terminal will be locked in this case, exit the gui application or software, then terminal will be opened , use & , after name of software so that terminal , agar chat he ki termi khuli rahe aur soft chlta rahe, toh & bhi barte saath mein , hum apni tarf se kuch bhi path bana toh sakte hain par linux mein jab vo chalega toh error aa jayega kyunki apne jo khud se folder name diye hain vo exixst nhi karte, agar PATH mein bhi  karoge toh bhi, export mein bnhi, solution pehle mkdir -p se random path banadein fir varibale bana dein export ya nano karke kaam ke hi saab se, iske baad jab bhi aap karoge toh aaram se vo khul jayegam ye sab custom env se sambhav ha
version check karne ke liye , -v aur --v ka chakkar zyada nhi hai, java kjaise purane soft ke kaaran -v use hota hai, agar vers chec karn ha, pa pata na kaa likhe,toh man ya help command use kar sakat he ya -v air--v dono type kare
emv variables vo hote jinmein variable mein kuch information store ki hoti hai, ye humare system ki diary hoti hai, hum jo bhi kaam karte hain, system diary mein dekhta hai, agar usse vo mil jaata hai toh output mil jaata hai, agar vahan vo information nhi hai toh error aa jaata hai ya kuch nhi hota, inmein har ek information store nhi hoti jaise user name, permissions, home name, names , system ki information vagiara, jo computer ko chalane mein help karti hain vo hi sab cheezein hoti hain , agar koi file ya information humari kisi drive mein hai toh hum uska path variable banakar save zarooor kar sakte aur usse terminal mein open karke dekh bhi sakte hain, bas itna hai kihumein usse define karna padta hai export se for tempo and nanobashrc for permanent, kyunki computer mein pehle se sab kuch nhi hota, isiliye hum apni require ke hisab se batadete ya define karte hain ki is information ko bhi apni diary mein note karlo. simple .....///, ab aaap path banayegenge , system mein nayi cheezein add karenge toh delete bhi karni hongi taaki ram full na ho, toh hum unset command use karte hain, hum bas variable ka naam likh dete hain aur unset command daalte hi , vo innfo delete ya remove ho jaati hai syst se, kabhi home mein reh kar seddha unset path mat karna kyunki isse system apne saare path ko hi delete kar deta hai aur baad mein jab aaap kuch comm, chalaoge toh nhi chelga , agar aisa kabhi hota hai toh ye ....PATH.... command use karein isse aapke basic commands sab activate ho jayenge, par agar aapne alag se variables banaakr kuch add kiya hua tha toh vo ismein nhi ayega, aur haan agar aapne bashrc mein path delte kar diya tha toh vahan par hi theek karna hoga , taaki permanent save ho PATH, agar terminal se command chlayo thi, toh upar wali command chalyein theek ho jyayega , agar aap apne dusri soft, info, ya file, fold, ko bhi vaapis laana chat hain toh ya toh linux ka bacshrc backup file check karein, ya fir export PATH: likh kar aage apna path jodkar us ko vahan par rakh sakte hain dubara se, agar folder apni marzi se name dekar banane hain toh mkdir se pehle folder bana dein isse appka system fir se unhe save kar lega aur app chala paoge flutter, java etc, ko bash rc mein likhna hoga par agar aapki bashrc kharab ya corrupt ho jaaye tph aap isse aise karke jo real default bashrc hai usmein jaakar saara code copy karke dubara se basgrc mein daal sakte hain jisse bilkul fresh file dubara ready ho jyegi, aap real skel bashrc mein changes nhi laa sakte, par apni copy basgrc mein laa sakte hain, aur jo bhi path soft,info purane mein thi, is nayi mein dubara daal kar save kar lijiye, bashrc kabhi bhi export path ka bcakup nhi rakhta kyunki vo banaya hi tempo hota hai, toh backup aur permanent ke liye real bachrc mein likh dein saara path......./etc/skel/.bashrc ~/.bashrc  ,read karein, cat /etc/skel/.bashrc
bhai, version chnage karte waqt pehle ek variable baan lein jaise ..., aur usko path ke saath, jismein vo real change waala version hai saath jodein isse vo varoable mein save ho hua, iske baad ... karke usse daal dein, ab aapko pura path nhi likhna pada aapne bas varibale name likha aur uske baad ...path likhein aisa isliye kyunki version chnage ke waqt pehle path desribe hota hai. softeware ke naam ke saane hum var nhi kar sakte, vahan humein path se hi save karna padta hai, env variable soft ya version ke waqt kaise aur kahan banana hai :
agar software installed hai pehle se , apt command se installed kiya hua hai toh, seedha software ka naaam daal kar enter dabayein soft terminal mein khul jayega , humein paths unke banane padte hain jo amnully download kiye gaye hain jaise java,flutter, sdk,etc. aur jo package manager ke custom tools ya fir kuch secret information jaise database, api keys, etc. inke liye sabse pehle naya path banayein , which ya whereis command se check karkefir purana path jod dein, database aur api keys ke liye sirf normally variable banakar store karein, iske ilava softwares ke versions chnage karne ke liye pehle naya version path jodein aur baad mein purana taaki aapp naye version ko use kar sakein. jab hum software ko terminal mein khilte hain toh vahan par save karne ka koi tarika  nhi hota humare kaam ko isliye professinals pehle vs code ya nano chalakar usmein code likhte hain aur file banate hain aur baad mein usse run kar dete hain python mein aur output dekh lete hain file banakr rakhne se code ssd mein save ho jaata hai file mein ,software bas test ke liye aur output paane ke liye hota hai. 







# Comprehensive Guide to Environment Variables & Package Management in Ubuntu

## 📖 Introduction to Environment Variables (ENVs)

Environment variables are key-value pairs that store essential configuration data about your system. Think of them as a **system diary** where information about executable applications and paths is kept. 

Whenever you run a command or perform an operation, Ubuntu checks these variables to see if the command exists and where it is located. 
* If the command is registered in the variables, the system executes it and shows the output.
* If it is not found, you will get a **command error** or execution failure.

---

## 🔍 Commands to Locate Executable Paths

Before working with environment variables, you often need to find where a specific software or command is installed on your system.

### 1. The `which` Command
This command is used to print the exact path of any executable command or application.

* **Syntax:**
  ```bash
  which <command_name_or_software>
  ```
* **Example:**
  ```bash
  which ls
  ```
* **Expected Output (If executable exists):**
  It will print the exact binary path.
  *📌 [Yahan apna Pehla Screenshot lagayein - which ls wala]*

* **Expected Output / Error (If executable does not exist):**
  If you check a software that isn't installed (e.g., `which java`), it will return an empty line or an error because the application is missing from the system.
  *📌 [Yahan apna Dusra Screenshot lagayein - which java wala]*

> ⚠️ **Note:** Errors or empty outputs can also happen due to a typo in the command name, wrong syntax, or when older versions of applications are replaced by newer ones.

### 2. The `whereis` Command (Recommended)
The `whereis` command is much more helpful than `which`. It does a broader search and provides additional information, such as the binary path, manual guide (`man` pages) path, and source/service paths all at once.

* **Syntax:**
  ```bash
  whereis <command_name_or_software>
  ```
* **Example:**
  ```bash
  whereis python3
  ```
* **Expected Output:**
  *📌 [Yahan apna Tisra Screenshot lagayein - whereis python3 wala]*

---

## 🛠️ Installing Missing Applications and Commands

If a software or command is not found using `which` or `whereis`, you need to install it first.

### Using the `sudo apt` Command
In Ubuntu, you use the Advanced Package Tool (`apt`) to install software directly from the terminal. The `sudo` command is written before `apt` because installing software requires administrative (**ROOT**) privileges. The system will ask for your login password to proceed.

* **Syntax:**
  ```bash
  sudo apt install <application_or_software_name>
  ```

> 💡 **Important Note:** When you install an application or command using the `apt` package manager, **you do not need to add its path manually** to the system. Ubuntu automatically creates and configures the paths for you. You can verify this immediately after installation by running the `which` or `whereis` command.

---

## 🚀 Creating Custom Environment Variables

If you want to create a new environment variable to store custom information (like API keys or specific text), you can use the `export` command.

### The `export` Command Syntax
```bash
export VARIABLE_NAME="value"
```

### Usage Rules:
1. **No Spaces:** Always write `KEY="value"`. Putting spaces around the `=` sign (e.g., `KEY = "value"`) will throw a syntax error.
2. **Naming Convention:** By convention, always write variable names in **UPPERCASE** (e.g., `DATABASE_URL` instead of `database_url`).



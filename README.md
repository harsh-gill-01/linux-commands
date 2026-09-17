# Linux Commands 

## My Linux Commands And Bash Scripts Notes 
## Basic Commands 

* `ls` - To list all the contents of our current directory. **Syntax**: `ls`
```bash
ls
```
**Expected Output:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/be73df06-9236-432f-9fa1-e12a1ee15256" />

---

* `pwd`- To check in which directory or location we are in current time.
**Syntax:**
`pwd`
```bash
pwd
```
**Expected Output:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ff1b54b0-3440-41a6-b55b-320d0baead12" />

---

* `clear` - To clear our terminal. You can also use `CTRL + L` to clear your terminal faster than `clear` command. 
**Syntax:**
clear
```bash
clear
```
**Expected Output:** 

<img width="600" alt="image" src="https://github.com/user-attachments/assets/c0f237ca-438d-4ad2-8515-e07cb842b0c6" />

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ff21990b-b45d-4f31-89c9-29f4394134ce" />

---

* `date` - To check date, along with time, timezone etc.
**Syntax:**
date
```bash
date
```
**Expected Output:**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/ba21578d-6138-46fb-853f-be55d65f16d5" />

---

* `touch` - To create a file in linux.
**Syntax:**
`touch [file name]` **Example:**
touch my_file
```bash
touch my_file
```
**Expected Output:**

<img width="500" alt="image" src="https://github.com/user-attachments/assets/4d1d143b-53d9-451d-92b8-2135d3469925" />

---

* `mkdir` - To create a folder.
**Syntax:**
`mkdir [folder name]` **Example:**
`mkdir my_folder`
 
```bash
mkdir my_folder
```
**Expected Output:**

<img width="500" alt="image" src="https://github.com/user-attachments/assets/6ef15c28-a0c7-41f3-a9c2-41a8b09342e0" />

---

* `rm` - To delete a file.
**Syntax:**
`rm [file name]` **Example:**
`rm my_file`

```bash
 rm my_file
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/35679bfb-04c4-4e3b-b5cd-f4e85d9fc905" />

---

* `rm -rf` - To delete a folder. You can also use `rmdir` command for the same purpose.
**Syntax:**
`rm -rf [folder name]` **Example:**
`rm -rf my_folder`

```bash
rm -rf my_folder
```
**Syntax:**
`rmdir [folder name]` **Example:**
`rmdir newfolder`

```bash
rmdir newfolder
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/6c50249e-afd1-4158-a3f6-4d4a2385aa5e" />

---

* `cal` - To see calendar of current year or month, we can also see calendars of past or future years along with months by writing year number and month name.
**Syntax:**
`cal` **Example:**
`cal`

```bash
cal
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/b0842ee6-a334-47b6-9005-d9fbfa6c3faa" />

---

* `ls -lt` - To see all the information about our files and folders of current directory. It provides all the information about the files and folders , about their sizes , their  creation time & date etc.
**Syntax:**
`ls -lt`
```bash
ls -lt
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/3abdee9a-c169-4bb6-b2b1-9e522f25313a" />

---

* `ls -ltr` - To see all the information about our files and folders of current directory in reverse order. Reverse order of our contents shows us the very new files and folders that we created new.
**Syntax:**
`ls -ltr`  
```bash
ls -ltr
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/23cdab4f-e224-4a1b-86c1-f529ba25ddf9" />

---

* `ls -lh` - To see information about our files and folders in a manner to make them more easier to read. In this command , `h` means human readable.
**Syntax:**
`ls -lh`
```bash
ls -lh
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/7b0d13cd-8d37-4bd7-b66d-d8059613889e" />

---

* `bc` - To open a calculator like system in your terminal to do basic calculations. Generally, you will not get a proper visible calculator in your terminal. You will just get a platform in your terminal after executing command to perform basic calculations. Press `ctrl + D` to come back from calculator to terminal.
**Syntax:**
`bc` 
```bash
bc  
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/552a061d-745f-48af-8a8a-0532db518221" />

---

* `--help` - To get help regarding a command. You will write before this command , the command about which you want to get help.
**Syntax:**
`[command name] --help` **Example:**
`ls --help` 

```bash
ls --help
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/24dd95f5-3a79-45d7-a280-ac82d06b64a0" />

---

* `man` - To get manual regarding a command. This command shall help you , but will provide its manual also. Like, giving every information regarding its uses, use cases , syntax , etc. Press `Q` to come out.
**Syntax:**
`man`
**Example:**
`man ls`
```bash
man ls
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/121c2e92-1727-4c92-b243-7b585fa03f68" />

---

* `cd` - Use this command to change directory or for surfing in multiple folders and directories . You can also use `/` for going or moving in multiple folders by describing path. This command will let you access directories of current location. Never forget to give name of the directory and folder in which you want to go and access. Use this command alone , means without giving any name of folder or directory to get return yourselves back to home directory (~ home directory). Directories or folders appear different in color. 
**Syntax:**
`cd [folder or directory name]` **Example:**  `cd folder`

```bash
cd folder
```
**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/fc7fa4bb-0b3c-43d2-8db0-03a85c31e485" />

---

* `whoami` - To know about who you are in this terminal. When you will use this command , it will return your user name through which you are logged in and using. This `id` command will return some other information like your id,uid etc.
**Syntax:**
 `whoami` 
```bash
whoami
```
```bash
id
```
**Expected Output:**

<img width="500" alt="image" src="https://github.com/user-attachments/assets/8c596326-7135-4241-8bac-efb0f41bf657" />

---

* `uptime` - Use this command to check that how many users are logged in or using this terminal, time from which terminal is open or from in use, load on terminal .
**Syntax**
`uptime`  
```bash
uptime
```
**Expected Output:** 

<img width="400" alt="image" src="https://github.com/user-attachments/assets/35204fe9-0a3d-4811-b6ab-708bcdb1d4a3" />

---

* `cd ../` - Use this command to go back one directory from current location. You can use multiple slashes as per the number of folders or directories you are in to go back. In the **Expected Output**, i went to `folder` , then `newfolder` , then i went back one folder by using `cd ../` , then i went two folders back by `cd ../../` command , then i went upto `folderA` by describing its path from `home` folder .
**Syntax:**
* `cd [folder name]` - to go inside a folder.
* `cd ../` - to go back one directory.
* `cd ../../` - To go back two directories.
* `cd ////` - by describing path between slashes you can access your required folder.

**Example:**
`cd folder`
`cd newfolder`
` cd ../`
`cd ../../`
`cd folder/newfolder/folderA`
 
```bash
cd folder
cd newfolder
cd ../
cd ../../
cd folder/newfolder/folderA
```

**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/43305944-3f0c-495f-9a74-8b5f279e0c39" />

---

* `mv` - To move files and folders from one directory to another in linux. We should give the name of files and folders which we want to move .  It moves the files and folders to the desired directories. You can also change name of files and folders. We can also use `mv ../ [file or folder name]` command to get any folder or file in current directory or folder without going back.
**Syntax:**
* `mv [file name] [folder or directory].`
* `mv [folder or directory name] [folder or directory name].`
* `mv ../[file or folder name].` You can get any file or folder from any previous folders or directories without going back by using number of `../` as per the location of files or folders.
* `mv [file or folder name] [file or folder name] for changing name.`

**Example:**
`mv fileB my_folder`
`mv folder mynewfolder` 
`mv ../filenew .`
`mv file_A file_AA`
`mv folder FOLDER`

```bash
mv fileB my_folder
mv folder mynewfolder 
mv ../filenew .
mv file_A file_AA
mv folder FOLDER
```

**Expected Output:**

<img width="600" alt="image" src="https://github.com/user-attachments/assets/eba6ae55-e775-4f90-824f-ec954a4d56d3" />

---

* `cp` - to copy files and their content. The name of the file should be written by us after the command which we want to copy.
**Syntax:**
* `cp [file name] [folder or directory].`
* `cp [file name] [another file name].` (for copying only content of one file to another file).
* `cp ../[file name] .` You can get any file and its content from any previous folders or directories without going back by using number of `../` as per the location of files or folders.
* `cp [file name] [file name] .` For copying the content as well as creating new copy of file from another name.

**Example:**

`cp FILE new_folder`
`cp FILE file_new`
`cp ../fileC .`
`cp file_new new_File`

```bash

cp FILE new_folder
cp FILE file_new
cp ../fileC .
cp file_new new_File

```

**Expected Output:**

FIRST TWO COMMANDS : 

<img width="600" alt="Screenshot 2026-09-13 120616" src="https://github.com/user-attachments/assets/019ded80-8a35-471e-a5be-bbcfa9d61e5f" />

LAST TWO COMMANDS :

<img width="600" alt="Screenshot 2026-09-13 121310" src="https://github.com/user-attachments/assets/88e72df8-29f9-4a50-b6b8-33de27e63e92" />

---

* `cat` - to read a file.
**Syntax:**
`cat [file name]`

**Example:**
 `cat FILE`
   
```bash
cat FILE
```
**Expected Output:**

<img width="500" alt="image" src="https://github.com/user-attachments/assets/e0eb7c18-fea6-4a1e-84bb-379bd1d71796" />

---

* `less` - to read a file. It provides some other options comparing to cat command for better and proper reading and finding some important or specific words in files. In this, the big files will be opened in another editor or reader of files not in your terminal.

**NOTE:**
  
In this, the files will be opened in another editor or reader of files not in your terminal. For reading BIG files there are some helpful things you can do. Press `/` and write the specific word or name , anything you want to read in file that your file contains, this is for searching and reading from top to bottom. Press `?` and write specific name or word you want to read in the file for searching or reading information from bottom to top. After using `/` and `?` for searching specific information from top to bottom and bottom to top, press `N` for seeing more or same like that information you searched. If there will be same or more information about your search it will show you, and when it will be finished, it will return `Pattern not found (Press Return)`. Press `Q` to quit file reading and come back to the terminal. Press `SHIFT + G` to go down at the last line of the file and press `P` to go up to the first line.
  
**Syntax:**
`less [file name]`

**Example:**
`less file`
`less fileB`

```bash
less file
less fileB

```
**Expected Output:**

Output of Smaller File (file)
<img width="895" height="871" alt="Screenshot 2026-09-14 124048" src="https://github.com/user-attachments/assets/5e83c81d-388a-4977-ad3e-3f022e631394" />
Execution of Bigger File (fileB)
<img width="400" alt="Screenshot 2026-09-14 124404" src="https://github.com/user-attachments/assets/3fdd1856-cb9f-414e-90c9-6592bdff44a0" />

Output of Bigger File (fileB)
<img width="500" alt="image" src="https://github.com/user-attachments/assets/84e2ac39-7acf-4c39-9d32-4c14a3933996" />

This Is How You Will Search specific information with `/` `?`
<img width="896" height="871" alt="Screenshot 2026-09-14 124546" src="https://github.com/user-attachments/assets/8779c41a-b356-422e-937b-e14a9ac08fb7" />
<img width="892" height="875" alt="Screenshot 2026-09-14 124631" src="https://github.com/user-attachments/assets/5cb522c6-265a-4b9a-8bd9-96fbbbe88dbc" />

---

* `more` - To read a file page by page and word or line by line. Press `ENTER` to read line by line and `Down Arrow` to read page by page (it will scroll down more than 4-5 lines of file). In this , your file is opened in your terminal , not in another file reader. But for big files, you will have to press `Q` to quit file reading as same as with `less` command. The above written reading thing will work only if your file is big, it will not work upon small files as usual. It also shows the percentage of file you've read, like this way `--More-- (70%)`, as you will use `down arrow` and scroll the file you will automatically come out when you will have finished it to the end, this is due to opening of your file reader in terminal, not an editor or separate reader like `less` command.

**Syntax:**
`more [file name]`

**Example:**
`more fileC`
`more fileB`

```bash
more filec
more fileB
```
**Expected output:**

Output of Smaller File (fileC)
<img width="887" height="452" alt="image" src="https://github.com/user-attachments/assets/ffd5900e-f2eb-44e4-bf0e-175fea7ed90a" />

Execution of Bigger File (fileB)
<img width="893" height="240" alt="image" src="https://github.com/user-attachments/assets/2b02a7c4-96e6-49c9-b98e-9ef89c6166c1" />

Output of Bigger File (fileB)
<img width="891" height="873" alt="image" src="https://github.com/user-attachments/assets/cd960e68-86d9-4375-a826-c1048128c7b6" />

---

* `nano` - To edit a file very perfectly. It provides many options to edit a file as per our requirements. Its benefit is, you dont need to create a file first by using `touch` command. It will create file as well as will provide options to edit the file.
```bash
nano fileB
```
* `vi` - to edit a file. Press insert after entering into the editor, and start editing it by writing text or any other things.
```bash
vi myfile
```
* `grep` - It's full form is **Global Regular Expression Print**. Used To search words in files. It will return on your terminal all the words containing that file. 

**Syntax:**
`grep 'word' [file name]`

**Use cases:**



**Example:**
`grep 'A' fileB`

```bash
grep 'A' fileB
```
**Expected Output:**

<img width="896" height="192" alt="image" src="https://github.com/user-attachments/assets/d4977845-fcfb-4e35-b8e0-c805ea63e914" />

---

* `egrep` - To search multiple words and information in files. Write the name of the file and use pipe or vertical bar (|) for searching multiple words at a time.

**Syntax:**
`egrep `words or information` [file name]`
```bash
egrep A|G|H|J|C| my_file
```
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

how to describe and write path for setting an env for a software or application :

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

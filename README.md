# Linux Commands 

## My Linux Commands And Bash Scripts Notes 
## Basic Commands 

* `ls` - To list all the contents of our current directory.
**Syntax:**

```bash
ls
```
**Expected Output:**

<img width="500" height="260" alt="image" src="https://github.com/user-attachments/assets/be73df06-9236-432f-9fa1-e12a1ee15256" />
---

* `pwd`- To check in which directory or location we are in current time.
**Syntax:**
pwd
```bash
pwd
```
**Expected Output:**

<img width="400" height="164" alt="image" src="https://github.com/user-attachments/assets/ff1b54b0-3440-41a6-b55b-320d0baead12" />
---

* `clear` - To clear our terminal. You can also use `CTRL + L` to clear your terminal faster than `clear` command. 
**Syntax:**
clear
```bash
clear
```
**Expected Output:** 

<img width="600" height="314" alt="image" src="https://github.com/user-attachments/assets/c0f237ca-438d-4ad2-8515-e07cb842b0c6" />
<img width="400" height="219" alt="image" src="https://github.com/user-attachments/assets/ff21990b-b45d-4f31-89c9-29f4394134ce" />
---

* `date` - To check date, along with time, timezone etc.
**Syntax:**
date
```bash
date
```
**Expected Output:**

<img width="400" height="178" alt="image" src="https://github.com/user-attachments/assets/ba21578d-6138-46fb-853f-be55d65f16d5" />
---

* `touch` - To create a file in linux.
**Syntax:**
touch
**Example:**
touch my_file
```bash
touch 
```
**Expected Output:**

<img width="500" height="197" alt="image" src="https://github.com/user-attachments/assets/4d1d143b-53d9-451d-92b8-2135d3469925" />
---

* `mkdir` - To create a folder.
**Syntax:**
mkdir
**Example:**
mkdir new_folder 
```bash
mkdir 
```
**Expected Output:**

<img width="500" height="187" alt="image" src="https://github.com/user-attachments/assets/6ef15c28-a0c7-41f3-a9c2-41a8b09342e0" />
---

* `rm` - To delete a file.
**Syntax:**
rm
**Example:**
rm new-file
```bash
 rm 
```
**Expected Output:**

<img width="600" height="246" alt="image" src="https://github.com/user-attachments/assets/35679bfb-04c4-4e3b-b5cd-f4e85d9fc905" />
---

* `rm -rf` - To delete a folder. You can also use `rmdir` command for the same purpose.
**Syntax:**
rm -rf
**Example:**
 rm -rf my-folder
```bash
rm -rf 
```
**Syntax:**
rmdir
**Example:**
rmdir newfolder
```bash
rmdir
```
**Expected Output:**

<img width="600" height="330" alt="image" src="https://github.com/user-attachments/assets/6c50249e-afd1-4158-a3f6-4d4a2385aa5e" />
---

* `cal` - To see calendar of current year or month, we can also see calendars of past or future years along with months by writing year number and month name.
**Syntax:**
cal
**Example:**
cal sep 2026
```bash
cal
```
**Expected Output:**

<img width="600" height="376" alt="image" src="https://github.com/user-attachments/assets/b0842ee6-a334-47b6-9005-d9fbfa6c3faa" />
---

* `ls -lt` - To see all the information about our files and folders of current directory. It provides all the information about the files and folders , about their sizes , their  creation time & date etc.
**Syntax & Example:**
ls -lt
```bash
ls -lt
```
**Expected Output:**

<img width="600" height="759" alt="image" src="https://github.com/user-attachments/assets/3abdee9a-c169-4bb6-b2b1-9e522f25313a" />
---

* `ls -ltr` - To see all the information about our files and folders of current directory in reverse order. Reverse order of our contents shows us the very new files and folders that we created new.
**Syntax:**
ls -ltr  
```bash
ls -ltr
```
**Expected Output:**

<img width="600" height="752" alt="image" src="https://github.com/user-attachments/assets/23cdab4f-e224-4a1b-86c1-f529ba25ddf9" />
---

* `ls -lh` - To see information about our files and folders in a manner to make them more easier to read. In this command , `h` means human readable.
**Syntax:**
ls -lh 
```bash
ls -lh
```
**Expected Output:**

<img width="600" height="753" alt="image" src="https://github.com/user-attachments/assets/7b0d13cd-8d37-4bd7-b66d-d8059613889e" />
---

* `bc` - To open a calculator like system in your terminal to do basic calculations. Generally, you will not get a proper visible calculator in your terminal. You will just get a platform in your terminal after executing command to perform basic calculations. Press `ctrl + D` to come back from calculator to terminal.
**Syntax:**
bc 
```bash
bc  
```
**Expected Output:**

<img width="600" height="499" alt="image" src="https://github.com/user-attachments/assets/552a061d-745f-48af-8a8a-0532db518221" />
---

* `--help` - To get help regarding a command. You will write before this command , the command about which you want to get help.
**Syntax:**
--help
**Example:**
ls --help  
```bash
--help
```
**Expected Output:**

<img width="600" height="870" alt="image" src="https://github.com/user-attachments/assets/24dd95f5-3a79-45d7-a280-ac82d06b64a0" />
<img width="600" height="878" alt="image" src="https://github.com/user-attachments/assets/817f539e-d106-4cee-b260-f6fe564253a0" />
---

* `man` - To get manual regarding a command. This command shall help you , but will provide its manual also. Like, giving every information regarding its uses, use cases , syntax , etc. Press `Q` to come out.
**Syntax**
  man
**Example:**
man ls
```bash
man 
```
**Expected Output:**

<img width="600" height="868" alt="image" src="https://github.com/user-attachments/assets/121c2e92-1727-4c92-b243-7b585fa03f68" />
---

* `cd` - Use this command to change directory or for surfing in multiple folders and directories . You can also use `/` for going or moving in multiple folders by describing path. This command will let you access directories of current location. Never forget to give name of the directory and folder in which you want to go and access. Use this command alone , means without giving any name of folder or directory to get return yourselves back to home directory (~ home directory). Directories or folders appear different in color. 
**Syntax:**
cd
**Example:**  
cd folder
```bash
cd
```
**Expected Output:**

<img width="600" height="353" alt="image" src="https://github.com/user-attachments/assets/fc7fa4bb-0b3c-43d2-8db0-03a85c31e485" />
---
* `whoami` - To know about who you are in this terminal. When you will use this command , it will return your user name through which you are logged in and using. This `id` command will return some other information like your id,uid etc.
**Syntax:**
 whoami 
```bash
whoami
```
```bash
id
```
**Expected Output:**

<img width="500" height="286" alt="image" src="https://github.com/user-attachments/assets/8c596326-7135-4241-8bac-efb0f41bf657" />
---

* `uptime` - Use this command to check that how many users are logged in or using this terminal, time from which terminal is open or from in use, load on terminal .
**Syntax**
uptime  
```bash
uptime
```
**Expected Output:** 

<img width="400" height="173" alt="image" src="https://github.com/user-attachments/assets/35204fe9-0a3d-4811-b6ab-708bcdb1d4a3" />
---

* `cd ../` - Use this command to go back one directory from current location. You can use multiple slashes as per the number of folders or directories you are in to go back. In the expected output, i went upto `newfolder` from home directory (~), I was in `~`, went to a folder named `folder` of `~` and then went to `newfolder` from `folder`, and then i went back two folders, and reached `~` home directory back.
**Syntax:**
cd ../
**Example:**
cd ../ & cd ../../../   
```bash
cd ../
```
**Expected Output:**

<img width="600" height="421" alt="image" src="https://github.com/user-attachments/assets/1d5519ea-f893-4fc2-a378-643e4c825e0e" />
<img width="400" height="135" alt="image" src="https://github.com/user-attachments/assets/132bd8df-9d07-408a-b4cb-2c1b85090702" />
---

* `mv` - To move files and folders from one directory to another in linux. We should give the name of files and folders which we want to move . It moves the files and folders to the desired directories.
```bash
mv file myfolder
```
* `cp` - to copy files and their content. The name of the file should be written by us after the command which we want to copy.
```bash
cp newfile myfolder
cp newfile NEWFILE
```
* `cat` - to read a file.
```bash
cat myfile
```
* `less` - to read a file. It provides some other options comparing to cat command for better and proper reading and finding some important or specific words in files.
```bash
less new_file
```
* `more` - to read a file page by page and word or line by line. Press enter to read line by line and down arrow to read page by page.
```bash
more fileA
```
* `nano` - to edit a file very perfectly. It provides many options to edit a file as per our requirements. Its benefit is, you dont need to create a file first by using `touch` command. It will create file as well as will provide options to edit the file.
```bash
nano fileB
```
* `vi` - to edit a file. Press insert after entering into the editor, and start editing it by writing text or any other things.
```bash
vi myfile
```
* `grep` - to search a word in files. Its used for searching of a word in files. Write the name of the file after the command while executing.
```bash
grep file_new
```
* `egrep` - to search multiple words and information in files. Write the name of the file and use pipe or vertical bar (|) for searching mutiplw words at a time.
```bash
egrep A|G|H|J|C| my_file
```
* `history` - use this command get all the history of your used command on terminal, use `history` command for getting all the commands history that are executed on the terminal till date. You can use `history |grep` command also to search a specific or single command name that you have executed on your terminal. The word grep is used here because it is used for searching only a single word. 
```bash
history
history |grep ls
```
* `gzip` - use this command to zip a file. It will compress your file and will give you the compressed version of your big file , thus helping us to share or store them easily. There will also be the real file along with compressed version. If you somehow remove the real file , then you can recover from compressed version by using `gunzip` or `gunzip -d` command. Write the name of the file you want to compress or decompress. While decompressing the file , write name of your compressed version file ( .gz , at the end ).
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

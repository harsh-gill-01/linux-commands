# Linux Commands 

## My Linux Commands And Bash Scripts Notes 
## Basic Commands 

* `ls` - to list all the contents of our current directory.
 ```bash
  ls myfiles folder1 fileA fileB
```
* `pwd`- to check in which directory or location we are in current time.
 ```bash
  /home/harsh
```
* `clear` - to clear our terminal.
 ```bash
  clear
```
* `date` - to check date.
 ```bash
  date
```
* `touch` - to create a file in linux.
 ```bash
  touch new_file
```
* `mkdir` - to create a folder.
 ```bash
  mkdir server_logs
```
* `rm` - to delete a file.
 ```bash
  rm mynewfile
```
* `rm -rf` - to delete a folder.
 ```bash
  rm -rf mynewfolder
```
* `cal` - to see calendar of current year or month, we can also see calendars of past or future years along with months by writing year number and month name.
 ```bash
  cal
```
* `ls -lt` - to see all the information about our files and folders of current directory. It provides all the information about the files and folders , about their sizes , their  creation time & date etc.
```bash
  ls -lt
  ```
* `ls -ltr` - to see all the information about our files and folders of current directory in reverse order. Reverse order of our contents shows us the very new files and folders that we created new.
 ```bash
  ls -ltr
  ```
* `ls -lh` - to see information about our files and folders in a manner to make them more easier to read. In this command , h means human readable.
 ```bash
   ls -lh
   ```
* `bc` - to open a calculator like system in your terminal to do basic calculations. Generally, you will not get a proper visible calculator in your terminal. You will just get a platform in your terminal after executing command to perform basic calculations.
```bash
 bc  
```   
* `--help` - to get help regarding a command. You will write before this command , the command about which you want to get help.
  ```bash
   ls --help
  ```
* `man` - to get manual regarding a command. This command shall help you , but will provide its manual also. Like, giving every information regarding its uses, use cases , syntax , etc.
```bash
man ls
```
* `cd` - use this command to change directory or for surfing in multiple folders and directories .You can also use / for going or moving in multiple folders by describing path. This command will let you access directories of current location. Never forget to give name of the directory and folder in which you want to go and access. Use this command alone , means without giving any name of folder or directory to get return yourselves back to home directory.
 ```bash
cd myfolder
cd myfolder/newfolder
``` 
* `whoami` - to know about you are in this terminal. When you will use this command , it will return your user name through which you are logged in and using. It will return some other information like your id,uid etc.
```bash
whoami
```
* `uptime` - use this command to check that how many users are logged in or using this terminal, time from which terminal is open or from in use, load on terminal .
```bash
uptime
```
* `cd ../` - use this command to go back one directory from current location. You can use multiple slashes as per the number of folders or directories you are in to go back.
```bash
cd ../
```
* `mv` - to move files and folders from one directory to another in linux. We should give the name of files and folders which we want to move . It moves the files and folders to the desired directories.
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
* `nano` - to edit a file very perfectly. It provides many options to edit a file as per our requirements. Its benefit is, you dont need to create a file first by using touch command. It will create file as well as will provide options to edit the file.
```bash
nano fileB
```
* `vi` - to edit a file. Press insert after entering into the editor, and start editing it by writing text or any other things.
```bash
vi myfile
```

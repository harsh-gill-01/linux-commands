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
* `find ./` - this command is used to find files. This is helpful because we can have a number of files in different folders or directories and we can not remember all of them. If we remember even the first letter of our file we can it with its path, means that where it is located, in which folder it is. We can use a wildcard also `*` before and after the files of name while finding them. Example - think of that you have a file named File.txt , but you do not know where it is then you use `find ./` command or even wildcard `*`.
```bash
**syntax**
find ./-name (name of file)
find ./-name new-file
find ./*.txt
``` 



# **LINUX FUNDAMENTAL**
- `Linux` is a unix-like operating system.
    - `unix-like` operating system is one that behaves in a manner similar to a unix system. although not being conforming to or being certified to any version of the single `unix` specifitions.

- why `linux`
    - `linux` is free.
    - `linux` is well-maintained.
    - `linux can run on any electronic machine like fridge, car, phone etc.
    - `ubuntu` is a linux distribution.

## **WHAT IS CLI**
- `CLI` stand for 
    - command line interface.
    - command line interpreter.
    - command line input.

- `CLI` is a command line program that accepts input to execute operating sytem functions.

## **SERVER**
- a `server` is a computer program or a device that provides a service to another computer program and its users known as `clients`.

- In a data center, the physical computer that a server program runs on is also frequently referred to as a `sever`.


## **DISTRO**
- a linux distribution (abbreviated as distros) is an operating system made from a software collection that includes the linux kernel, and often a package management system.

- Ex. `ubuntu`.

## **SHELL**
- The `shell` is a command line interface to your computer.

## **INTRO TO SHELL**
- `A terminal` is essentially a text-based user interface for interacting with computers. It allows user to execute commands and view the results, as well as control application running on the computer.

- `An interface` is a shared boundary across which two or more components of a computer system exchane information.
- ` a console` traditionally refers to a computer terminal where a user may input commands and view the output such as the result of the inputed commands or status message from the computers.
- `an emulator` is hardware or software that enables one computer syetem(called the **host**) to behave like another computer system (called the **guest**).
- `REPL: READ EVALUATE PRINT LOOP`
    - whatever is written on the console will be read first and then evaluated and then will be printed finally and this repl loop will continue infinitely.

## **SHELL SCRIPT**
- a shell script is a text-file that contains a sequence of commands for a unix-based operating system.

## **LINUX COMMAND**
- for any **linux commands** you can check the usage and different input flags it expects by running the command followed by **--help**.

- `pwd`: this represents what is thendirectory we are currently at.
- `ls`: you can print the content of the current directory we are in. All the files and sub-directories will be printed.
- `cd`: this can help you move into a folder and move out of a folder.
    - `cd ..`: if you want to jump one folder back from the current directory.

    - `cd ../..`:  if you want to make two jumps back from the current directory.
    - `cd ~`: from any directory this will help you to come back to the home directory.
    - `cd directory1/directory2/`: we can move into internal sub-directories directly by separating them with a forward slash (/).
    - `cd /`: from any directory, this will help you to come back to the root directory.
- `ls`: you can print the content of the current directory. All the files and folders are printed.
    - `ls -l`: list down more details about the file such as owner, permissions, data etc.

    - `ls -lh`: works like **ls -l** but also gives the size of the files.
    - `ls -a`: also lists files and folders starting with `.`.
- `clear`: clear the working space by actually moving you to the top of the current shell.
- `mkdir`:  this helps us to create a new folder.
- `touch <file-name>`: we can create a brand new blank file out of the blue.
- `cat <file-name>`: prints the whole consent of a file.
- `rm <file-name>`: delete the files permanently.
- `rmdir <folder>`: delete the folder permanently if folder is empty.
- `rm -r <folder-name>`: the **-r** flag enables rm to recursively delete all the content of the folder and then delete the folder.
- `rm -rf subfolder`: delete the folder either empty or not.
- `rm -rf/ ` : delete the root folder and hence all the critical files will be deleted and hence operating system will become corrupt.
- `tail <file-name>`: print the some last lines of the file on the consle.
- `tail -n 3 <file-name>`: print the last 3 lines of the file on the console.
- `tail -f <filename>`: this will print the some last lines of the file on the console without exiting the file. `ctrl+c`: karne par file exit ho jayega.
- `head file-name`: print the some first lines of the file on the consle.
- `head -n 10 file-name`: print  first 10 lines of the file on the consle.
- `cat`: print the whole file.
- `head` and `tail`: print part of the file on the console.
- `echo`: print the given statement/ strings on the console.
- `echo "sanket singh" > dump.txt`: sanket singh ko dump.txt file me dump kar dega. console pe kucch bhi print nhi hoga.
- `>`: This angular bracket is a command which will dump the command written on the left side of it to the file written on the right side of it.
- `ls | grep Dsa`: grep command is used to find the folder and files containing the string given after grep command.
- `|`: this is called piping. left side me command ke output ko right side ke command ko as an input deta hai.
- `ps aux`: it prints detail of all the processes running on our computer system currently.
- `ls > new.txt`: whatever is the result of ls will be dumped into new.txt, nothing will be printed on the console. if new.txt has some content already then that will be replaced.
- `ls>>new.txt`: whatever is the result of ls will be dumped into new.txt, nothing will be printed on the console. if new.txt has some content already then that will not be replaced, new content will be appended.
- `command1 && command2`: this executes command1 followed by command2 considering command1 has no errors.
- `cp file1 file2`: copies the content of file1 to file2.
- `mv file1 file2`: move (cut paste) the file1 to a new position as file2. This also help us to rename a file.
- `tar -cf archive.zip 1.txt 2.txt`: this command will compress all the files mentioned after archive.zip into the zipped archive as mentioned.
- `tar -zcf archive.zip 1.txt 2.txt`: this command will not only add the files to a zip but also compress them.
- `tar -xf archive1.zip -C extract`: all the content of the archive1 will be extracted out into extract folder.

- linux terminal by default gives the access of text-editor that are available in terminal by itself.
    1. vim
    2. nano

### **VIM**
- **vim** is a text editor available in linux terminal.

- `vim newfile.txt` or `vi newfile.txt`: 
    - if this file exists, vim will open it.
    - if it doesn't exists, it will create one and open it.
- **how to exit vim**:
    - ` :q`: will exit out of vim.
- vim can open files in multiples modes.
    1. `insert mode`: in this mode you can write something in the file.

    2. `normal mode`: you can move within the file but cannot make changes to it. you can read and navigate.
    3. `command mode`: you can execute some commands.
- by default, vim opens in normal mode.
- if you press `i` then from normal mode you will go into insert mode.
- if you want to exit the vim without saving the changes, just press ` :q!`
- if you want to exit the vim by saving the changes just command ` :wq`.

#### **VIM COMMANDS**
- ` vim filename`: 

    - this will create a file (if it doesn't exits) and then openn it in the vim editor in the normal mode.

    - In normal mode we cannot do changes to the file but we can read it and navigate it. You can also use `vi filename` to do the same.
    - now after opening vim if you want to start making changes you need to first of all make it change from normal to insert mode. To go in the insert mode, you can press `i`. If you want to come back to the normal mode then press `esc`.
    - `esc +:q`: if you need to exit a file we can do this.
    - `esc +:q!`: if file has some changes and we want to exit without saving changes.
    - `esc+:wq`: if file has changes and we want to save it and then exit.
    - `l`: in normal mode, you can move cursor right.
    - `h`: in normal mode, you can move cursor left.
    - `j`: in normal mode, you can move cursor down.
    - `k`: in normal mode, you can move cursor up.
    - you can use normal right, left, up and down arrow keys as well to navigate.
    > vim advenute is a game. Play it to learn vim shortcuts.
- `dd`: in **normal mode**, it will delete the line the cursor is currently at.
- `gg`:  in **normal mode**, it will make the cursor go on the first line.
- `G`: in **normal mode**, it will make the cursor go on the last line.
- `w`: in **normal mode**, it can make the you jump one word.
- `2w`: in **normal mode**, it can make you jump 2 word.
- `d2w`: this will delete 2 words.
- `yw`: in **normal mode**. it copies one word.
- `yy`: in **normal mode**, it copies a whole line.
- `p`: for pasting in normal mode.
- `%s/old word/new word/`: replaces old word with new word.
- if you want to change the layout of vim file, you can open vimrc file and update it.
    - `vim ~/.vimrc`: syntax to open vimrc file.

    
### **Note:**
- `~`: this **tilda** refers to the home directory. Ex: /user/rahul.
- `/`: this slash leads you to the root directory.
- `Relative path`: It describes the location of a file/folder w.r.t. current folder.
- `Absolute path`: 
    - In an absolute path we mention the location from home directory to root directory.
    - when you give the absolute path of a file or a folder that means you will give the whole path of that file or folder, whereas in the relative path you do jump w.r.t to the current folder.


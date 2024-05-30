# 0x00. Shell, basics

This was an introduction to shell basics and the concepts learnt were: the shell, navigation, a tour of the Linux file system, manipulating files with commands such as mv, cp, rm and many more, scripting, keyboard shortcuts and many more.

## Resources

1). [What is "the Shell"?](https://linuxcommand.org/lc3_lts0010.php)

2). [Navigation](https://linuxcommand.org/lc3_lts0020.php)

3). [Looking around](https://linuxcommand.org/lc3_lts0030.php)

4). [A Guided Tour](https://linuxcommand.org/lc3_lts0040.php)

5). [Manipulating files](https://linuxcommand.org/lc3_lts0050.php)

6). [Working with commands](https://linuxcommand.org/lc3_lts0060.php)

7). [Reading man pages](https://linuxcommand.org/lc3_man_pages/man1.html)

8). [Keyboard shortcuts for Bash](https://www.howtogeek.com/181/keyboard-shortcuts-for-bash-command-shell-for-ubuntu-debian-suse-redhat-linux-etc/)

9). [LTS](https://wiki.ubuntu.com/LTS)

10). [Shebang](https://en.wikipedia.org/wiki/Shebang_%28Unix%29)


## Tasks

**Task 0:**
[0-current_working_directory](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/0-current_working_directory)- Write a script that prints the absolute path name of the current working directory.
![1](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/f8ae8d39-11a3-4875-a0ab-92d1a6b6cf47)

**Task 1:**
[1-listit](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/1-listit)- Display the contents list of your current directory. ![2](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/cc3616b9-c872-4d16-9599-17923df99af1)

**Task 2:**
[2-bring_me_home](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/2-bring_me_home)- Write a script that changes the working directory to the user’s home directory. You are not allowed to use any shell variables.


![3](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/4d424d32-94b6-47db-86bd-2663af86964d)

**Task 3:**
[3-listfiles](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/3-listfiles)- Display current directory contents in a long format. ![4](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/5c0b2dda-ed89-420c-a147-88e6160ae79e)

**Task 4:**
[4-listmorefiles](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/4-listmorefiles)- Display current directory contents, including hidden files (starting with .), use the long format. ![5](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/b57a0739-37ad-4659-bd63-5eaf3e4b1f9d)

**Task 5:**
[5-listfiles-digitsonly](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/5-listfilesdigitonly)- Display current directory contents: long format, with user and group IDs displayed numerically and hidden files (starting with .) 


![6](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/a5d1cc2e-081f-4b95-967b-9f1b7a09685a)

**Task 6:**
[6-firstdirectory](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/6-firstdirectory)- Create a script that creates a directory named my_first_directory in the /tmp/ directory. ![7](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/d381d4fa-aeb1-4555-8b1c-55dc29d34d24)

**Task 7:**
[7-movethatfile](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/7-movethatfile)- Move the file betty from /tmp/ to /tmp/my_first_directory.![8](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/ab28fd33-2ae7-4357-beee-efdd8c9e54f1)

**Task 8:**
[8-firstdelete](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/8-firstdelete)- Delete the file betty in /tmp/my_first_directory.![9](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/bb16c8e6-baf2-43e5-90b9-21154ff5ff92)

**Task 9:**
[9-firstdirdeletion](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/9-firstdirdeletion)- Delete the directory my_first_directory that is in the /tmp directory.![10](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/08ff5da4-8ac0-4739-a1b0-b16f6b356d86) 

**Task 10:**
[10-back](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/10-back)- Write a script that changes the working directory to the previous one. ![11](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/158519ee-d0ba-481c-aa81-4a60dccca95c)

**Task 11:**
[11-lists](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/11-lists)- Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format. ![12](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/cc0c3079-d88a-401f-94a0-e3b9aef12d0d)

**Task 12:**
[12-file_type](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/12-file_type)- Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.


![13](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/f049b5df-1cf8-41df-aa40-12ed1e9596e4)

 **Task 13:**
[13-symbolic_link](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/13-symbolic_link)- Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory. 

![14](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/2ca67d39-e663-4b98-a55b-a68a66b27896)
 
 **Task 14:**
 [14-copy_html](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/14-copy_html)- Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory. You can consider that all HTML files have the extension .html ![15](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/70ceabc4-92fe-42ba-ab29-af8222541780)

 **Task 15:**
 [100-lets_move](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/100-lets_move)- Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u. You can assume that the directory /tmp/u will exist when we will run your script.![16](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/dfb3af72-d17e-4c17-a657-2a90202e58a2)
 
 **Task 16:**
 [101-clean_emacs](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/101-clean_emacs)- Create a script that deletes all files in the current working directory that end with the character ~. ![17](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/a9addbbf-aed6-47cf-add5-ca222a10324e)

 **Task 17:**
 [102-tree](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/102-tree)- Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory. You are only allowed to use two spaces (and lines) in your script, not more. ![18](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/70bef217-3701-47a4-81ac-a4db1a1f0756)

 **Task 18:**
 [103-commas](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/103-commas)- Write a command that lists all the files and directories of the current directory, separated by commas (,). ![19](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/51df3628-b590-415e-834f-e4bdc5e43fda)
 
 **Task 19:**
[school](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x00-shell_basics/school) Create a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0. 
**Note:** school.mgc is created using file -C -m school
![20](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/ff39271c-6d22-43a2-8169-a55a7f0ecd79)


 
 

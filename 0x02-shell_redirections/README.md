# 0x02. Shell, I/O Redirections and filters

This covered Linux shell I/O Redirections for standard output, error and input, filters, pipelines and metacharacters. Commands learnt about include echo, cat, head, tail, fins, wc, sort, uniq, grep, sort, tr, rev, cut and passwd.

## Resources

1). [Shell, I/O Redirection](https://linuxcommand.org/lc3_lts0070.php)

2). [Special characters](https://mywiki.wooledge.org/BashGuide/SpecialCharacters)

3). [Chapter 6 of 'The Linux command line'](https://linuxcommand.org/tlcl.php)

## Learning Objectives

**Shell, I/O Redirection**

- What do the commands head, tail, find, wc, sort, uniq, grep, tr do
- How to redirect standard output to a file
- How to get standard input from a file instead of the keyboard
- How to send the output from one program to the input of another program
- How to combine commands and filters with redirections

**Special Characters**
- What are special characters
- Understand what do the white spaces, single quotes, double quotes, backslash, comment, pipe, command separator, tilde and how and when to use them

**Other Man Pages**
- How to display a line of text
- How to concatenate files and print on the standard output
- How to reverse a string
- How to remove sections from each line of files
- What is the /etc/passwd file and what is its format
- What is the /etc/shadow file and what is its format

## Tasks

**Task 0**: [0-hello_world](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/0-hello_world)- Write a script that prints “Hello, World”, followed by a new line to the standard output.
![0](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/c29a8e32-974a-45e3-8280-c499198b85e6)

**Task 1**: [1-confused_smiley](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/1-confused_smiley)- Write a script that displays a confused smiley "(Ôo)'.
![1](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/40ad6438-4612-4860-9ee7-87d47b13298b)

**Task 2**: [2-hellofile](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/2-hellofile)- Display the content of the /etc/passwd file.
![2](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/d17024e0-b768-49b2-907f-5eec9fef0770)

**Task 3**: [3-twofiles](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/3-twofiles)- Display the content of /etc/passwd and /etc/hosts files.
![3](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/a77591b6-823f-42f3-bd5e-3a65764a5364)


**Task 4**: [4-lastlines](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/4-lastlines)- Display the last 10 lines of /etc/passwd.
![4](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/2c6fdd5d-47fc-4f20-91cb-6ad64de8560f)


**Task 5**: [5-firstlines](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/5-firstlines)- Display the first 10 lines of /etc/passwd.
![5](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/d86229ac-c751-47aa-8724-b81e334494e3)

**Task 6**: [6-third_line](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/6-third_line)- Write a script that displays the third line of the file iacta.
![6](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/410b4d9b-fe2c-43ed-99fd-5fe53b0045d0)


**Task 7**: [7-file](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/7-file)- Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.

![7](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/e9684ba6-5cd6-4250-9888-fa655291e95d)


**Task 8**: [8-cwd_state](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/8-cwd_state)- script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
![8](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/51d21eeb-7c44-4e88-b6d6-0b1b23fbab41)

**Task 9**: [9-duplicate_last_line](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/9-duplicate_last_line)- Write a script that duplicates the last line of the file iacta.
![9](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/adf7c1fa-7fba-494c-a10b-0b76da010b47)

**Task 10**: [10-no_more_js](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/10-no_more_js)-script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
![10](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/678ea5af-5164-4684-89b5-d6c86d9e8b33)

**Task 11**: [11-directories](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/11-directories)- Write a script that counts the number of directories and sub-directories in the current directory. The current and parent directories should not be taken into account. Hidden directories should be counted.
![11](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/d38b230a-637a-425b-8513-dd952353dd15)

**Task 12**: [12-newest_files](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/12-newest_files)- script that displays the 10 newest files in the current directory.
![12](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/2d3effe8-bd3c-4bd8-a0f2-507cbcc1f8be)

**Task 13**: [13-unique](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/13-unique)- Create a script that takes a list of words as input and prints only words that appear exactly once.
![13](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/3f150950-e31c-49a3-8932-834c0ff100b9)

**Task 14**: [14-findthatword](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/14-findthatword)- Display lines containing the pattern “root” from the file /etc/passwd
![14](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/730894a8-9888-4c24-aff0-7e01c959b4f1)

**Task 15**: [15-countthatword](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/15-countthatword)- Display the number of lines that contain the pattern “bin” in the file /etc/passwd
![15](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/68b7a3fa-a762-4e11-841c-2c53a00abb81)

**Task 16**: [16-whatsnext](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/16-whatsnext)- Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.
![16](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/05296d41-2f20-45f9-b03e-23b1c0822bdd)

**Task 17**: [17-hidethisword](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/17-hidethisword)- Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.
![17](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/c806f120-3571-412c-b220-5ee046ffa7ef)

**Task 18**: [18-letteronly](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/18-letteronly)- Display all lines of the file /etc/ssh/sshd_config starting with a letter, include capital letters as well.
![18](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/cb522abd-df90-4fa9-8b47-6fac6d00f3d1)

**Task 19**: [19-AZ](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/19-AZ)- Replace all characters A and c from input to Z and e respectively.
![19](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/726b1b73-0bfd-4f83-a707-ed3405ea0e77)

**Task 20**: [20-hiago](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/20-hiago)- Create a script that removes all letters c and C from input.
![20](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/7281796a-8572-4f44-9fa5-5d861b2c2449)

**Task 21**: [21-reverse](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/21-reverse)- Write a script that reverse its input
![21](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/2a524739-25b9-406c-aaf8-7ee956487ee3)

**Task 22**: [22-users_and_homes](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/22-users_and_homes)- Write a script that displays all users and their home directories, sorted by users, based on the the /etc/passwd file

![22](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/5f4c8d5f-b1d9-4d93-8722-66290b2ec127)

**Task 23**: [100-empty_casks](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/100-empty_casks)- Write a command that finds all empty files and directories in the current directory and all sub-directories.
Only the names of the files and directories should be displayed (not the entire path)
![23](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/25dcb665-1cd3-42bc-8728-d5a8868bdf65)

**Task 24**: [101-gifs](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/101-gifs)- Write a script that lists all the files with a .gif extension in the current directory and all its sub-directories.
Hidden files should be listed.
![24](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/dc8556ac-ff8e-43d2-b456-5c8a82c9a5da)

**Task 25**: [102-acrostic](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/102-acrostic)- Create a script that decodes acrostics that use the first letter of each line.
![25](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/9f0a0c2e-a9e8-413a-80ed-682c41f3db3f)

**Task 26**: [103-the_biggest_fan](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x02-shell_redirections/103-the_biggest_fan)- Write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
![26](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/dfe21665-63bc-4b23-b6c6-2b7a6d4eca1b)



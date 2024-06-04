# 0x03. Shell, init files, variables and expansions
This is a continuation of shell and bash scripting that looks at expansions(tilde, parameter, arithmetic, brace, pathname, command substitution), quoting, escaping characters, shell arithmetic(shell expansion, compound command, let built-in, declare -i), variables(global/environment, local/shell), special parameters($*, $@, $-, $_, $$, $0, $!, $#) and alias command.

## Resources
1. [Expansion](https://linuxcommand.org/lc3_lts0080.php)
2. [Shell arithmetic](https://www.gnu.org/software/bash/manual/html_node/Shell-Arithmetic.html)
3. [Variables](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_02.html)
4. [Shell initialization files](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_01.html)
5. [Alias](https://www.linfo.org/alias.html)
6. [Technical Writing](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2021/6/9112669886fd446a2aa3113c31319d1f468dc160.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240604%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240604T000430Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=689a626dea90437f329f1c495508f3609f05b1cbeafb0d9aeaf7ba24a1430862)
7. man pages of printenv, set, unset, export, alias, unalias, source/. and printenv.

## Tasks
**Task 0:** [0-alias](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/0-alias)- Create a script that creates an alias. 
Name: ls
Value: rm *
![0](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/1660cf73-b19e-42ac-aacb-df83e2fd560e)

**Task 1:** [1-hello_you](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/1-hello_you)- Create a script that prints hello user, where user is the current Linux user.
![1](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/cbaa0dce-38b9-4bf1-9602-fb1de3534a22)

**Task 2:** [2-path](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/2-path)- Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
![2](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/22aed9fd-69f9-46ba-a8e3-7b95be757b59)

**Task 3:** [3-paths](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/3-paths)- Create a script that counts the number of directories in the PATH.
![3](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/748471ee-af41-4939-96d8-7bf2acafe396)

**Task 4:** [4-global_variables](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/4-global_variables)- Create a script that lists environment variables.
![4](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/b056d9d3-4b3b-4490-b3d4-62b444e03979)

**Task 5:** [5-local_variables](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/5-local_variables)- Create a script that lists all local variables and environment variables, and functions.
![5](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/592a58a9-c36a-49db-bdc8-ecf1a6adf0ce)

**Task 6:** [6-create_local_variable](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/6-create_local_variable)- Create a script that creates a new local variable.
![6](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/be54e31a-ae85-4f7b-900a-e718893cfdce)

**Task 7:** [7-create_global_variable](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/7-create_global_variable)- Create a script that creates a new global variable.
![7](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/93252ff8-5cfa-47d4-8c4b-d034e0b07c26)

**Task 8:** [8-true_knowledge](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/8-true_knowledge)- Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.
![8](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/71a40ee7-d25f-4d7e-83fc-94b9f031338c)

**Task 9:** [9-divide_and_rule](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/9-divide_and_rule)- Write a script that prints the result of POWER divided by DIVIDE, followed by a new line. POWER and DIVIDE are environment variables.
![9](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/b8fb132f-e85d-40dd-af00-641348210cca)

**Task 10:** [10-love_exponent_breath](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/10-love_exponent_breath)- Write a script that displays the result of BREATH to the power LOVE. BREATH and LOVE are environment variables.
![10](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/6f9b1bfa-ed08-4c99-8813-abe8c4623c2e)

**Task 11:** [11-binary_to_decimal](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/11-binary_to_decimal)- Write a script that converts a number from base 2 to base 10. The number in base 2 is stored in the environment variable BINARY. The script should display the number in base 10, followed by a new line.
![11](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/85957ced-0104-4480-9ce5-86da2945dc5d)

**Task 12:** [12-combinations](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/12-combinations)- Create a script that prints all possible combinations of two letters, except oo.
![12](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/d5d05d91-f202-4f47-9e88-299bd7fa0505)

**Task 13:** [13-print_float](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/13-print_float)- Write a script that prints a number with two decimal places, followed by a new line. The number will be stored in the environment variable NUM.
![13](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/8d7d11d3-12c1-4525-aefa-b37a6afba8de)

**Task 14:** [100-decimal_to_hexadecimal](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/100-decimal_to_hexadecimal)-Write a script that converts a number from base 10 to base 16. The number in base 10 is stored in the environment variable DECIMAL. The script should display the number in base 16, followed by a new line 
![14](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/dac4f21a-b545-4149-b701-ffe41569b420)

**Task 15:** [101-rot13](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/101-rot13)- Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII.
![15](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/60aa2087-82ac-4f7f-adfa-5a9f20431293)

**Task 16:** [102-odd](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/102-odd)- Write a script that prints every other line from the input, starting with the first line.
![16](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/fc6b2db3-2e2a-47b3-8508-ac483a283020)

**Task 17:** [103-water_and_stir](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/blob/main/0x03-shell_variables_expansions/103-water_and_stir)- Write a shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result. WATER is in base water. STIR is in base stir.The result should be in base bestchol.
![17](https://github.com/Muthoni-Maryanne/alx-system_engineering-devops/assets/107298263/d9ad92d0-883c-4b45-b470-e0698194e621)


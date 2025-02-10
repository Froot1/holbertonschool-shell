<p align="center">
<img width="520" align="center" altlt="Image" src="https://github.com/user-attachments/assets/e4685b2b-eb52-4a3c-a638-52ef1da8f96e" />
</p>

# Shell, I/O Redirections and filters

* [Task 0](./0-hello_world): Write a script that prints “Hello, World”, followed by a new line to the standard output. **echo Hello, World**
* [Task 1](./1-confused_smiley): 1 Write a script that displays a confused smiley "(Ôo)'. **echo "\"(Ôo)'"**
* [Task 2](./2-hellofile): Display the content of the /etc/passwd file. **cat /etc/passwd**
* [Task 3](./3-twofiles): Display the content of /etc/passwd and /etc/hosts. **cat /etc/passwd /etc/hosts**
* [Task 4](./4-lastlines): Display the last 10 lines of /etc/passwd. **tail /etc/passwd**
* [Task 5](./5-firstlines): Display the first 10 lines of /etc/passwd. **head /etc/passwd**
* [Task 6](./6-third_line): Write a script that displays the third line of the file iacta. **head -3 iacta | tail +3**
* [Task 7](./7-file): Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line. **echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)"**
* [Task 8](./8-cwd_state): Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it. **ls -la > 'ls_cwd_content'**
* [Task 9](./9-duplicate_last_line): Write a script that duplicates the last line of the file iacta. **tail -n 1 iacta >> iacta**
* [Task 10](./10-no_more_js): Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders. **find . -type f -name "*.js" -delete**
* [Task 11](./11-directories): Write a script that counts the number of directories and sub-directories in the current directory. **find . -mindepth 1 -type d | wc -l**
* [Task 12](./12-newest_files): Create a script that displays the 10 newest files in the current directory. **ls -1t | head **
* [Task 13](./13-unique): Create a script that takes a list of words as input and prints only words that appear exactly once. **sort | uniq -u **
* [Task 14](./14-findthatword): Display lines containing the pattern “root” from the file /etc/passwd. **grep root /etc/passwd**
* [Task 15](./15-countthatword): Display the number of lines that contain the pattern “bin” in the file /etc/passwd. **grep -c bin /etc/passwd**
* [Task 16](./16-whatsnext): Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd. **grep -A 3 root /etc/passwd**
* [Task 17](./17-hidethisword): Display all the lines in the file /etc/passwd that do not contain the pattern “bin”. **grep -L bin /ect/passwd **
* [Task 18](./18-letteronly): Display all lines of the file /etc/ssh/sshd_config starting with a letter. **grep '^[A-Z | a-z]' /etc/ssh/sshd_config **
* [Task 19](./19-AZ): Replace all characters A and c from input to Z and e respectively. **tr A Z |tr c e**
* [Task 20](./20-hiago): Create a script that removes all letters c and C from input. **tr -d c | tr -d C **
* [Task 21](./21-reverse): Write a script that reverse its input. **rev**
* [Task 22](./22-users_and_homes): Write a script that displays all users and their home directories, sorted by users. **cat /etc/passwd | cut -d : -f 1,6 /etc/passwd | sort **
* [Task 23](./23-empty_casks): Write a command that finds all empty files and directories in the current directory and all sub-directories. **find . -empty -printf %f'\n'**
* [Task 24](./24-gifs): Write a script that lists all the files with a .gif extension in the current directory and all its sub-directories. **find . -type f -name "*.gif" -printf "%f\n" | LC_ALL=C sort -f | rev | cut -b 5- | rev **
* [Task 25](./25-acrostic): Create a script that decodes acrostics that use the first letter of each line. **cut -c 1 | paste -s -d ' ' | tr -d ' '**
* [Task 26](./26-the_biggest_fan): Write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests. **tail -n +2 | cut -f 1 | sort | uniq -c | sort -n -r | head -n 11 | cut -b 9-**


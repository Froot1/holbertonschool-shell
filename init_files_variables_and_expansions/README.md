# Shell, init files, variables and expansions
Each file here is a script that execute a basic command from the shell. 

* [Task 0](./0-alias) - Create a script that creates an alias. alias  ls="rm *"
* [Task 1](./1-hello_you) - Create a script that prints hello user, where user is the current Linux user. **echo hello $USER**
* [Task 2](./2-path) - Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program. **export PATH=$PATH:/action**
* [Task 3](./3-paths) - Create a script that counts the number of directories in the PATH. **echo $PATH | tr ":" "\n" | wc -l**
* [Task 4](./4-global_variables) - Create a script that lists environment variables. **printenv**

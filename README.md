This project is a simple UNIX-like command-line shell implemented in C. It supports essential shell functionalities such as command execution, piping, input/output redirection, command history, and basic built-in commands.

Features
Execute external commands with arguments

Support for input (<) and output redirection (>, >>)

Piped commands (|) execution

Built-in commands: cd, pwd, exit, and history

Command sequencing with ;

Logical command execution using && and ||

Command history management (stores last 200 commands)

Signal handling for graceful interruption (Ctrl+C)

Usage
Compile the source code:

bash
Copy
Edit
gcc -o unix_shell unix_shell.c
Run the shell executable:

bash
Copy
Edit
./unix_shell
Use the shell prompt (sh>) to enter commands.

Example commands
ls -l | grep ".c" > output.txt

cd /path/to/directory

cat < input.txt | sort | uniq >> output.txt

pwd

history

command1 && command2 || command3; command4

Project Structure
unix_shell.c: Main source code implementing the shell.

Handles parsing, execution, piping, redirection, built-in commands, and signal handling.

Dependencies
POSIX-compliant system (Linux, macOS)

GCC or compatible C compiler

Author
Arnob Sarker Partho


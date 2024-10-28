# Minishell
Minishell is a custom shell implemented in C that replicates key features of the bash shell. The goal of this project is to create a minimal, functional shell with a focus on understanding how a shell works at its core.

## Features

Interactive Prompt: Displays a prompt while waiting for commands.  
Command History: Maintains a history of commands during the session.  
Command Execution: Searches for and executes commands based on the PATH variable, or using absolute/relative paths.  
Built-in Commands:
- echo (with -n option)  
- cd (with a relative or absolute path)  
- pwd  
- export  
- unset  
- env  
- exit  

Quotes Handling:  
- Single quotes (') prevent interpretation of meta-characters.  
- Double quotes (") prevent interpretation of meta-characters except for $.

Redirection:
- < redirects input.
- \> redirects output.
- << reads input until a defined delimiter is encountered.
- \>> redirects output in append mode.

Pipes: Implements pipes (|), allowing the output of one command to be the input of the next.  
Environment Variables: Supports expanding environment variables ($), including the special variable $? for the exit status of the last executed command.  
Control Characters:
- Ctrl-C: Displays a new prompt.
- Ctrl-D: Exits the shell.
- Ctrl-\: No action (like in bash).

## Installation
Clone the repository.

To perform the initial setup of the project, you can run the following commands:

```bash
make
```

# 2 DAY CLI 06/01/2023
## Table of Contents
[What is Command Line Interface?](https://github.com/HexeCalibre/KodeGo/blob/master/DAY1CLI.MD#what-is-command-line-interface)

[Why Learn CLI?](https://github.com/HexeCalibre/KodeGo/blob/master/DAY1CLI.MD#why-learn-cli)

[PowerShell Set Execution Policy](https://github.com/HexeCalibre/KodeGo/blob/master/DAY1CLI.MD#powershell-set-execution-policy)

[Powershell Commands](https://github.com/HexeCalibre/KodeGo/blob/master/DAY1CLI.MD#powershell-commands)

## What is Command Line Interface?
>is a program on your computer where you can create
>files, run programs, and navigate through your folders and other files. It's called Terminal if you're using a Mac, and it's called >Command Prompt for Windows.

## Why Learn CLI?
> 1. You Gain Greater Control over System Functions
> 2. You can use NPM for Package Installs
> 3. You can utilize Git Version Control / Version Control System
> 4. You need it to use preprocessors, Task Runners, and Bundlers
> 5. It's for Local Backend Development

## PowerShell Set Execution Policy
### How to set PowerShell's Code Execution Policy into Unrestricted
```powershell
Set-ExecutionPolicy Unrestricted
or
-Set ExecutionPolicy to Unrestricted
or
Set-ExecutionPoIicy -ExecutionPolicy Restricted
or
-Set ExecutionPqLicy to Restricted
```
### How to check PowerShell's Code Execution Policy
```powershell
Get-ExecutionPolicy
//Show current execution policy
```
## Powershell Commands
| Command                            | Function                                               |
| ---------------------------------- | ------------------------------------------------------ |
| `clear` or `cls`                    | Clear the contents of the console window.              |
| `dir` or `ls` or `Get-ChildItem`     | Show the contents of the current directory.            |
| `dir -force` or `ls -force` or `Get-ChildItem -Force` | Show the contents of the current directory, including hidden folders. |
| `mkdir` or `md <folder name>`        | Create a new directory.                                |
| `cd <folder name>`                  | Open the specified directory.                          |
| `ni`                               | Create a new item.                                     |
| `ii`                               | Open a file or URL using the default program.           |
| `gc`                               | Get the content of a file.                             |
| `sc`                               | Set content in a file.                                 |
| `cd..`                              | Navigate to the parent directory (one level up).        |
| `cd ~`                             | Navigate to the user's home directory.                  |
| `ren <folder name>`                  | Rename a folder or file.                               |
| `del <folder name>`                  | Delete a directory or file.                            |
| `copy <source> <destination>`        | Copy a file or directory to a specified destination.    |
| `move <source> <destination>`        | Move a file or directory to a specified destination.    |
| `kill <process ID>`                  | Terminate a running process with the specified process ID. |
| `Get-Help <command>`                 | Get help documentation for a specific command.          |
| `Get-Alias`                         | Get a list of all defined aliases.                      |


Please note that these commands are commonly used in command-line interfaces like Windows Command Prompt or PowerShell.


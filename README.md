🐚 Custom Shell in C++
📘 Project Overview

This project was developed as part of the Capstone Project (Assignment 2) for the Linux Operating System course.
It is a console-based custom shell implemented in C++, designed to mimic basic Bash functionality — including command execution, process management, redirection, and piping.

🎯 Objectives

Execute standard Linux commands directly from the shell.

Manage foreground and background processes.

Support input/output redirection (>, >>, <).

Handle simple command piping (|).

Implement built-in commands: cd, jobs, and exit.

Gracefully handle process signals (e.g., background process completion).

⚙️ Features

✅ Execute standard commands (ls, pwd, date, echo, etc.)
✅ Manage background jobs using & and jobs command
✅ Input/output redirection (>, >>, <)
✅ Piping between two commands (|)
✅ Built-in commands: cd, exit, jobs
✅ Colored prompt showing current working directory
✅ Signal handling for process completion notifications

🧠 System Calls Used
Function	Purpose
fork()	Create a new process
execvp() / execv()	Execute an external program
waitpid()	Wait for a process to change state
open(), dup2(), close()	Handle file I/O and redirection
pipe()	Enable inter-process communication (piping)
signal()	Handle signals such as SIGCHLD for background process tracking

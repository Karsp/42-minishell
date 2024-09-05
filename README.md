# **Minishell - Build Your Own Bash-Like Shell**

Welcome to 💻 **Minishell**—a step forward of my previous project [Pipex](https://github.com/Karsp/42-pipex), where we take our journey with low-level programming to the next level by building a custom shell from scratch. This project teaches you to master **process management**, **file descriptors**, and **signal handling** in C, simulating a lightweight shell similar to Bash. 

If you’re passionate about systems programming and looking to deepen your understanding of how UNIX-like operating systems work under the hood, you’re in the right place! 🚀

## 📚 **Project Overview**

The goal of **Minishell** is to create a functional, user-interactive shell. This means implementing many of the core features that you use every day in your terminal, including command execution, piping, redirection, and more. The project allows you to get hands-on experience with how a shell processes commands, handles input/output, and manages processes—all critical concepts in low-level programming and operating systems.

### Example of Execution:
```bash
$> ./minishell
minishell$> ls -l | grep minishell
```

## 🧠 **Key Concepts and Knowledge Acquired**

- **Process Management & Forking**: You’ll work with system calls like `fork()` to create child processes, which is the backbone of multitasking in operating systems.
  
- **Pipes & Redirection**: Master the art of **pipes** (`|`) to connect the output of one command to the input of another, and handle input/output redirection (`<`, `>`, `>>`, `<<`), vital for controlling where data flows during execution.
  
- **Signal Handling**: Manage signals such as `ctrl-C`, `ctrl-D`, and `ctrl-\`, making your shell as interactive and responsive as Bash itself. This is critical for handling user inputs and process control in an interactive environment.
  
- **Environment Variables**: Learn how shells manage environment variables, expanding them dynamically during execution to provide a flexible user environment.
  
- **Built-in Commands**: Implement several key built-in commands like `echo`, `cd`, `pwd`, `export`, `unset`, `env`, and `exit`, giving you a deeper understanding of shell internal logic.

These concepts are foundational in **systems programming** and will help you become proficient in writing efficient, resource-conscious software that interacts directly with the OS.

## 🌟 **Features**

### Mandatory Part:
- **Interactive Shell**: Simulates Bash-like functionality, with a prompt awaiting user commands.
- **Command Execution**: Executes commands based on the PATH variable, as well as absolute or relative paths.
- **Redirection**: Supports input/output redirection (`<`, `>`, `>>`, `<<`).
- **Pipes**: Allows chaining commands using pipes (`|`).
- **Environment Variables**: Expands environment variables dynamically within the shell.
- **Signal Handling**: Properly handles `ctrl-C`, `ctrl-D`, and `ctrl-\` similar to Bash.
- **Built-in Commands**: Implements `echo`, `cd`, `pwd`, `export`, `unset`, `env`, and `exit`.

### Our Bonus Features:
- 🌳 **Binary Tree Data Structure**: Utilized to manage command parsing and execution, offering efficient structuring and traversal of command sequences.
- 🤖 **Automaton for Special Cases**: Implemented a finite automaton to handle specific shell parsing cases, such as managing quotes, escape characters, and other edge cases, ensuring accurate command interpretation.

## 🛠️ **How to Build and Run**

### Prerequisites
- **GCC** or any standard C compiler
- **Readline** if it is not included in your OS (sudo apt-get install libreadline6 libreadline6-dev)

### Steps:
1. Clone this repository:
   ```bash
   git clone https://github.com/Karsp/42-minishell.git
   ```

2. Navigate to the project directory:
   ```bash
   cd 42-minishell
   ```

3. Build the project using the provided `Makefile`:
   ```bash
   make
   ```

4. Run the shell:
   ```bash
   ./minishell
   ```

### Example Usage:
```bash
minishell$> echo "Hello World" > output.txt
minishell$> cat output.txt
minishell$> ls -la | grep minishell
```

## 🏗️ **Project Structure**
- **src/**: Contains all the source code files.
- **includes/**: Header files for function prototypes and macros.
- **Makefile**: Compiles the project and manages cleaning (clean, fclean), rebuilding (re), and bonus rules.

## 🎯 **Why This Project Matters**

By creating your own shell, you’ll gain an in-depth understanding of the following:
- **How shells manage commands and processes**, from basic execution to advanced process control.
- **File descriptors and redirection**: Learn how to manage multiple I/O streams efficiently.
- **Signal management**: Respond to system signals, a critical aspect of controlling user interactions in any shell.
- **Handling built-ins and environment variables**: Key components of shell functionality that allow flexible and dynamic command execution.

This project will take your **low-level programming** skills to new heights, as you'll be directly interacting with the underlying components of the OS. It’s a real test of efficiency, process management, and resource handling—all essential skills for any systems programmer.

## 📜 **License**
This project is open-source and available under the [MIT License](LICENSE).

---

Building **Minishell** is not only a step toward mastering C programming but also a journey into the heart of UNIX-based operating systems. It gives you a solid foundation for systems-level development, making you a stronger and more resourceful developer.

Feel free to explore the code and reach out with any questions!
```


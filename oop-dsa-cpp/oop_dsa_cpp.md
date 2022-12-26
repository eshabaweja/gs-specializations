# Object-Oriented Data Structures in C++

> University of Illinois at Urbana-Champaign

## Week 1

### Key Concepts

- C++ language syntax 
- Writing, compiling and debugging code 
- Interactive development environment (IDE) 
- C++ classes 
- Implementation v. header files 
- Public v. private elements of a class 
- Linking to external libraries to access helper routines 
- Namespaces

### About C++

- **strongly typed**: every variable has a type, name, value, and location in memory
- variables are of 2 types: `primitive` and `user-defined`

![image-20221226182224220](oop_dsa_cpp-assets/image-20221226182224220.png)

![image-20221226182238224](oop_dsa_cpp-assets/image-20221226182238224.png)

- :warning: The Standard Template Library in C++ (with the "std" namespace) **may be a standard library**, but the published standard only describes how it should work. The professor refers to it as "user-defined" because it **still needs to be implemented** by the creators of your operating system and compiler. Although it is standardized, it is built in the same way that you can define your own complex types and libraries.

- Every C++ program has a standard starting point: the  `main()` function.
- `int main()` must return integer values. By convention, `0 = success` and `non-zero = error `
- `std::cout` means output to console. `<<` shows concatenation.

### Linux-compatible system

- Not every operating system has the same collection of system functions and command-line environment, so in practice developing in C++ can be somewhat different depending on which operating system you are targeting. We'll use Linux.
- GNU/Linux: ersions, called "distributions"
- **Terminal/Shell/Command prompt**: They all refer to the text-based system management window that is used for typing system commands.
- Bash: This is one of the most common **text-based shell environments**.
- AWS Cloud9: This is a **web-based Linux terminal** you can set up, that is hosted on Amazon's AWS service. This is a good backup option for some users.
- The "sudo" part means this command will temporarily be executed with system administrator permissions. (The "su" part comes from **"superuser"**, which means system administrator. Other terms for this are "root user" or simply "administrator".) 
- A **symlink** (also called a **symbolic link**) is a type of file in Linux that  points to another file or a folder on your computer. Symlinks are  similar to shortcuts in Windows.
- create a symlink as: `ln -s <path to the file/folder to be linked> <the path of the link to be created>`
- https://www.freecodecamp.org/news/symlink-tutorial-in-linux-how-to-create-and-remove-a-symbolic-link/

### What is Git?

- "version control system"
- sites like GitHub offer hosting services for projects managed by the "git" software.
- https://github.com/wadefagen/coursera
- 

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
- You can use any of these editors for *editing your code text*, but for actually building (compiling), you need to use the **makefiles** that we provide. These are special scripts designed to work with the terminal program "Make", which is executed in the Bash terminal simply by typing **make**.
- https://opensource.com/article/18/8/what-how-makefile

### C++ Classes (User-defined types)

- classes encapsulate data and associated functionality into an object

![image-20221226220033907](oop_dsa_cpp-assets/image-20221226220033907.png)

- **protection levels** (public and private): decide the access that client code has to the member data or functionality
- private data and functions are only accessible inside the class
- **private** member variables have an **underscore** at the end of their name, like `length_`

- C++ **header file** `.h` defines the interface of the class whereas `.cpp` defines implementation
- `.h` contains **declaration** of all member variables and declaration of all member functions
- the `.cpp` file contains all the logic to implement our class
- `.h` files begin with `# pragma once` so that the class's definition is compiled only once
- class declaration also ends in a semicolon, just like primitive data types

![image-20221226220712771](oop_dsa_cpp-assets/image-20221226220712771.png)

### STD (Standard Library) vs STL

<table><thead><tr><th>STD</th><th>STL</th></tr></thead><tbody><tr><td>Std stands for standard</td><td>Stl stands for standard template library</td></tr><tr><td>Std falls under the standard C++ Library</td><td>Stl is a subset of std&nbsp;</td></tr><tr><td>All libraries fall under std.</td><td><p>There are 4 categories of stl:</p><ul><li>Algorithms</li><li>Functions.</li><li>Iterators</li><li>Containers.</li></ul></td></tr><tr><td>Space resolution operator is used(::)</td><td>No operator is used</td></tr><tr><td><p><strong>Examples:</strong>&nbsp;</p><p>cin, cout under iostream header</p></td><td><p><strong>Example:</strong></p><p>sort(),lower_bound().</p></td></tr></tbody></table>

- iostream header includes operations for reading/writing to files and console `std::cout`
- header files must be included as `#include <iostream>`

![image-20221226222640496](oop_dsa_cpp-assets/image-20221226222640496.png)

- A **namespace** is **a declarative region that provides a scope to the identifiers (the names of types, functions, variables, etc) inside it**. Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes  multiple libraries.

![image-20221226223043741](oop_dsa_cpp-assets/image-20221226223043741.png)

- do the above `namespace{class...}` enclosing in both `.h` and `.cpp`

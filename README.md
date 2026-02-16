# CPP Module 01 - Memory Allocation, Pointers to Members, and File Streams

This module focuses on the practical differences between **Stack** and **Heap** memory allocation in C++. It also explores the power of **Pointers to Members** and the basics of file manipulation using **C++ Streams**.



## 🧠 Key Learning Objectives

* **🟢 Memory Management**: Understanding the lifecycle of objects allocated on the Stack (automatic) vs. the Heap (manual using `new` and `delete`).
* **🔵 References vs. Pointers**: Learning when to use references for safety and pointers for flexibility.
* **🟡 Member Function Pointers**: Implementing dynamic function calling within a class to replace complex conditional logic.
* **🔴 File I/O**: Mastering the usage of `std::ifstream` and `std::ofstream` for reading and writing files.



## 📂 Exercise Breakdown

### 🟢 Ex00: BraiiiiiiinnnzzzZ
* **Goal**: Implement a `Zombie` class and understand two different creation methods.
* **Concepts**:
    * **`newZombie`**: Heap allocation for objects that must persist beyond the current scope.
    * **`randomChump`**: Stack allocation for temporary objects.
    * Identifying the exact moment of destruction via class destructors.

### 🟠 Ex01: Moar brainz!
* **Goal**: Allocate an entire "horde" of Zombies in a single call.
* **Concepts**:
    * **Array Allocation**: Using `new[]` to allocate memory for multiple objects.
    * **Batch Deletion**: Using `delete[]` to properly free allocated arrays and avoid memory leaks.

### 🔵 Ex02: HI THIS IS BRAIN
* **Goal**: Demystify the relationship between values, pointers, and references.
* **Concepts**:
    * Declaring and printing addresses and values of a `std::string`, a pointer to it (`stringPTR`), and a reference to it (`stringREF`).

### 🟣 Ex03: Unnecessary violence
* **Goal**: Manage object dependencies between a `Human` and their `Weapon`.
* **Concepts**:
    * **Member Types**: Deciding whether to store a class member as a pointer (if it can be NULL or change) or a reference (if it is constant and mandatory).

### 🟡 Ex04: Sed is for losers
* **Goal**: Create a program that replaces occurrences of a string within a file.
* **Concepts**:
    * **File Manipulation**: Opening, reading, and creating files using `<fstream>`.
    * **String Operations**: Utilizing `std::string::find()` and `std::string::replace()` logic.
    * Handling file errors (e.g., non-existent files or permission issues).

### ⚪ Ex05: Harl 2.0
* **Goal**: Implement a "Harl" object that complains at different levels (DEBUG, INFO, WARNING, ERROR).
* **Concepts**:
    * **Pointers to Member Functions**: Creating an array of function pointers to call specific level-methods without using an `if/else if` forest.
    * Improving code scalability and readability.

### 🔴 Ex06: Harl filter
* **Goal**: Filter Harl's output based on a minimum log level using `switch`.
* **Concepts**:
    * **Switch Case Fall-through**: Implementing a logic where a selected level triggers itself and all subsequent, more severe levels.
    * Command-line argument parsing and input validation.



## 🚀 Technical Requirements
* **Standard**: C++ 98.
* **Compiler**: `c++` with flags `-Wall -Wextra -Werror`.
* **Prohibited**: No `printf()`, `malloc()`, or `free()`. Use C++-style `std::cout`, `new`, and `delete` exclusively.
* **Memory Safety**: No memory leaks allowed. All heap-allocated objects must be properly deleted.


# happylearnCPP -- Programming Abstractions in C++ 
## Basic feeds
- g++.exe for .cpp files vs. gcc.exe for .c files
- Import library:
  - #include<libraryname> //a C++ system library
  - #include"libraryname.h" //a local project library

## Namespaces
- Standard namespace (std): 
   - std::cout<<"Text"<< var <<std::endl
- Define namespace
- Use namespace
    - using namespace name;  write below the #include
    - namespace::identifier  (std::)
    
## User input and output
- Console output: cout
- Console input: cin >> variable (Discouraged!)
  - #include "simpio.h"
    - getInteger("prompt") repeatedly prompts until an integer is typed; returns it
    - getReal("prompt") repeatedly prompts until double is typed; returns it
    - getLine("prompt") prompts and reads/returns an entire line of text
    - getYesOrNo("prompt")

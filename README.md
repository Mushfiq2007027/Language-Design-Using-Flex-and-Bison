# Language Design Project

## Description
This project demonstrates the design and implementation of a simple programming language using **C**.  
It involves lexical analysis, parsing, syntax tree construction, and interpretation.  
The aim is to showcase compiler design concepts and provide a working prototype of a custom language.

---

## Objectives
- Understand the process of designing a programming language.
- Implement lexical analysis to tokenize source code.
- Build a parser for syntactic structure analysis.
- Generate an Abstract Syntax Tree (AST).
- Interpret and execute programs written in the designed language.

---

## Features
- **Lexical Analysis:** Tokenizes input source code into meaningful symbols.
- **Parsing:** Checks for syntax correctness and constructs the AST.
- **AST Representation:** Data structure representing program structure.
- **Interpreter:** Executes the AST to produce output.
- **Error Handling:** Basic error messages for invalid syntax or tokens.

---

## Tools and Technologies
- **Language:** C  
- **Compiler:** GCC  
- **OS:** Windows / Linux  
- **Libraries:**
  - Standard C libraries: `stdio.h`, `stdlib.h`, `string.h`

---

## Components

| Component   | Description | Input | Output | Key Details |
|-------------|-------------|-------|--------|-------------|
| **Lexer**   | Scans the input source code and converts it into a sequence of tokens. | Source code string | List of tokens | Tokens: `IDENTIFIER`, `NUMBER`, `KEYWORD`, `SYMBOL`, `OPERATOR` |
| **Parser**  | Verifies syntactic correctness and constructs the AST based on grammar rules. | Tokens from lexer | Abstract Syntax Tree | Grammar: `<stmt_list> -> <stmt> | <stmt> <stmt_list>`<br>Statement Types: `assignment`, `print`, `loop`, `conditional` |
| **Interpreter** | Traverses the AST and executes the program. | Abstract Syntax Tree | Program output | Supports arithmetic (`+`, `-`, `*`, `/`), assignment, print, loops, conditionals |

---

## Usage
1. Write source code in the custom language syntax.
2. Run the compiler:
   ```bash
   ./my_lang <source_file>

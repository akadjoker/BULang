
# BU Lang

## Introduction

BU Lang is a simple, custom programming language inspired by Div Games Studio, developed to make game creation more accessible. This repository contains the source code for various components of the language, including the lexer, parser, interpreter, and more. This project aims to serve as an educational tool and a practical framework for game development.

## Components

- **Ast.py**: Contains the abstract syntax tree (AST) structures used by the parser and interpreter.
- **Interpreter.py**: Implements the interpreter for executing BULang programs.
- **Lexer.py**: Responsible for lexical analysis, breaking down the input source code into tokens.
- **Parser.py**: Implements the parser, which converts a sequence of tokens into an AST.
- **Printer.py**: Contains utilities for pretty-printing the AST and other structures.
- **Token.py**: Defines the token types used by the lexer.
- **Visitor.py**: Implements the visitor pattern for traversing the AST.
- **main.py**: The main entry point for running BULang programs.


### Examples

#### Program Structure

Structure of a BU Lang program:

```c
program name;
{
    // Your code here
}
```

#### Conditional Example

Example of using `if` in BU Lang:

```c
int score = 85
if (score >= 90) 
{
    print("Grade: A")
} elif (score >= 80) 
{
    print("Grade: B")
} else 
{
    print("Grade: C")
}
```

#### Switch Example

Here is an example of a switch statement in BULang:

```c
switch(value)
{
    case 0:
    {
        // Case 0 code
    }
    default:
    {
        // Default case code
    }
}
```

#### Loops Examples

Here are examples of different loops in BULang:

**For Loop:**

```c
for (int i=0; i<10; i=i+1)
{
    // Loop code
}
```

**While Loop:**

```c
while(i < 0)
{
    break;
    continue;
}
```

**Do-While Loop:**

```c
do
{
    break;
    continue;
} while(i < 10)
```

#### Process Example

Here is an example of defining and using processes in BULang:

```c
program name;
{
    start nave(100,100);
}

process nave(int _x, int y)
{
    int speed_x = 2;
    int speed_y = 2;
    x = _x;
    y = _y;

    loop // process loop
    {
        x = x + speed_x;
        y = y + speed_y;

        if (key(SPACE))
        {
            start bala(x, y + 5); // create new process
        }
    }
    // byebye nave, kill the process
}

process bala(int _x, int y)
{
    int speed_y = 2;
    x = _x;
    y = _y;

    loop
    {
        y = y - speed_y;

        if (y < 0)
        {
            break;
        }
    }
    // byebye bullet, kill the process
}
```

## Types 

- **int, float,string,bool**

- **TODO**
- **Struct**
- **Clases**
- **Bytecode**


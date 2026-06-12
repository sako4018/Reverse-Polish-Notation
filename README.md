# 🧮 RPN Calculator (C# Console Application)

A clean and interactive console calculator built in C# that evaluates mathematical expressions using Reverse Polish Notation (RPN) and a stack-based algorithm.

## 📌 Overview

This project implements a simple RPN evaluator. Instead of traditional infix notation (like `5 + 3`), it uses postfix notation such as `5 3 +`.

The program reads input from the console and outputs the result instantly.

## ⚙️ Features

- Supports basic arithmetic operations: `+`, `-`, `*`, `/`
- Stack-based evaluation system
- Interactive console input
- Error handling for invalid operators and insufficient operands
- Colored output for results (green)
- Continuous execution until `exit` command
- Console clears after each calculation

## 🧠 How It Works

The program uses a `Stack<double>`:

- Reads a line from the console
- Splits input into tokens
- If token is a number → pushes it to stack
- If token is an operator → pops two values, applies operation, pushes result back
- Final value in the stack is printed

## 🧪 Example

Input:
5 1 2 + 4 * + 3 -

Output:
14

Explanation:
1 2 + → 3  
3 4 * → 12  
5 + 12 → 17  
17 - 3 → 14  

## ⌨️ Usage

Run the project:
dotnet run

Type an expression in RPN format and press Enter.

To exit:
exit

## 🛠️ Tech Stack

- C#
- .NET Console Application
- Stack (`System.Collections.Generic`)

## 🚀 Purpose

This project was created to practice:
- Stack data structures
- Expression parsing
- Console applications in C#
- Algorithmic thinking

## 📄 License

Free to use

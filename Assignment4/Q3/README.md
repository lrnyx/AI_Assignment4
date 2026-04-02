# Sudoku Solver using CSP (Backtracking)

## Overview
This project implements a Sudoku Solver using Constraint Satisfaction Problem (CSP) techniques. It uses a backtracking algorithm to fill in missing values in a 9×9 Sudoku grid while satisfying all Sudoku constraints.

---

## Problem Description

Sudoku is a logic-based puzzle where:
- Each row must contain numbers from 1 to 9 (no repetition)
- Each column must contain numbers from 1 to 9
- Each 3×3 subgrid must contain numbers from 1 to 9

Empty cells are represented using `0`.

---

## Approach

The solution uses the Backtracking Algorithm:

1. Find an empty cell  
2. Try numbers from 1 to 9  
3. Check if the number is valid:
   - Not in the same row  
   - Not in the same column  
   - Not in the same 3×3 box  
4. If valid, place the number  
5. Recursively solve the rest  
6. If stuck, backtrack and try the next number  

---

## Functions Used

- print_board() → Prints the Sudoku board  
- find_empty() → Finds the next empty cell  
- is_valid() → Checks if a number can be placed  
- solve_sudoku() → Solves using backtracking  

---

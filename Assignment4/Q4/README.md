# Cryptarithmetic Problem Solver (TWO + TWO = FOUR)

## Overview
This project solves a cryptarithmetic puzzle using Python. Each letter represents a unique digit, and the goal is to find a valid digit assignment such that the equation TWO + TWO = FOUR holds true.

---

## Problem Description

Given the equation:

TWO + TWO = FOUR

Each letter corresponds to a unique digit from 0 to 9.

Constraints:
- No two letters can have the same digit
- Leading digits (T and F) cannot be zero
- The equation must be mathematically correct

---

## Approach

The solution uses brute-force with permutations:

1. Generate all possible digit permutations for the letters
2. Assign digits to letters (T, W, O, F, U, R)
3. Skip cases where T or F is zero
4. Convert letters into numbers:
   - TWO = 100*T + 10*W + O
   - FOUR = 1000*F + 100*O + 10*U + R
5. Check if TWO + TWO equals FOUR
6. Stop when a valid solution is found

---

## Concepts Used

- Brute Force Search  
- Permutations (itertools)  
- Constraint Satisfaction  


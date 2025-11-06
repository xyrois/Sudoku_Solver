# Sudoku Solver (Backtracking)

## Problem Description
The goal is to solve a 9×9 Sudoku puzzle**, where each row, column, and 3×3 box must contain all digits from 1 to 9 without repetition.  
Empty cells are represented by `0`s, and the task is to fill in the grid so that all Sudoku constraints are satisfied.

---

## Backtracking

1. Find the first empty cell (value `0`).
2. Try placing digits `1` through `9` in that cell.
3. For each number:
   - Check if it’s valid (not already in the same row, column, or 3×3 box).
   - If valid, place it and recursively attempt to solve the rest of the board.
   - If the recursion fails (no valid number can be placed later), backtrack by resetting the cell to `0` and try the next number.
4. The algorithm continues until all cells are filled correctly.

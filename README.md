# Mario-pyramid-block

# 🧱 Mario 

A C program that prints two side-by-side pyramids inspired by Super Mario. The user provides a height, and the program renders the double pyramid with a gap in between.

## 🔍 Example Output (height = 4)
Height: 3

      # # 
      
     ## ##
     
    ### ###

## 🚀 Features
- Prompts user for a non-negative integer height between 0 and 23 (inclusive).
- Validates input and reprompts until a legal height is given.
- Constructs two pyramids with correct spacing using nested loops.

## 🛠 Tech Stack
- **Language:** C  
- **Libraries:** `cs50.h` (for `get_int()`), `stdio.h`

## 🧠 How It Works (Algorithm Overview)
1. **Input Validation:** Prompt the user for a height and repeat until the input is an integer in the allowed range (0–23).
2. **Row Construction:** For each row from `0` to `height - 1`:
   - Print left padding (spaces) so the left pyramid is right-aligned.
   - Print `row + 1` hashes (`#`) for the left pyramid.
   - Print the fixed gap of two spaces.
   - Print `row + 1` hashes for the right pyramid.
   - Move to the next line.
3. **Nested Loops:** Uses nested `for` loops to control spaces and hashes per row, ensuring proper alignment.

## 📦 Files (example)
- `mario.c` – Source code implementing the More version of Mario.
- `Makefile` – Optional helper for compiling (`make mario`).
- `README.md` – This file.


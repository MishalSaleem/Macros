# Macros
# 🧵 8086 Assembly: Hello World using Macros

This 8086 Assembly program demonstrates how to use **macros** to print strings in a clean and reusable way. It prints `"Hello"` and `"World"` on separate lines.

---

## ✨ Features

- Uses **macros** (`string1`, `string2`) for repeated printing logic
- Prints:
![image](https://github.com/user-attachments/assets/9c844a9b-6d1f-4bb1-8fbd-536e9d6806fd)

# ➕ 8086 Assembly: Sum of Three Numbers Using Macros

This 8086 Assembly Language program demonstrates how to use **macros** to modularize and simplify code. It prompts the user to input **three single-digit numbers**, calculates their **sum**, and displays the result.

---

## 🧠 What It Does

1. Asks user for three single-digit inputs
2. Adds them together
3. Displays the sum using custom logic to convert numbers to ASCII

---

## 📦 Data Section

- `a`, `b`, `c` → Stores user input values
- `sum` → Stores the result (internally used in macro)
- Messages (`msg1` to `msg4`) → For prompts and output display

---

## 🧩 Macros Used

### 🔢 `Input`
- Prompts and takes 3 numeric inputs using `INT 21h`
- Stores them into `a`, `b`, and `c` after converting from ASCII

### ➕ `Sum`
- Adds `a + b + c`
- Stores result in `a`

### 📤 `Output`
- Converts the sum in `a` into ASCII digits
- Displays multi-digit sum using `push`/`pop` technique

---

## 💬 Sample Output
![image](https://github.com/user-attachments/assets/0f147408-934b-4729-9035-4bcf2d13877d)


# 🔠 8086 Assembly: String Length Calculator

This Assembly Language program reads a string from the user and calculates its length (number of characters) using **manual character counting**, then displays the result.

---

## 📋 Features

- Reads a string input from the user (up to 25 characters)
- Manually counts the number of characters
- Displays the calculated string length using interrupt-based output

---

## 🧩 Program Structure

### `.data`
- `st`: Stores the input string (up to 25 characters)
- `msg1`: Prompt message — "Enter String"
- `msg2`: Output label — "Length is"
- `len`: Stores the computed length

### `.code`
- `Input`: Reads characters until Enter (`carriage return`, ASCII 13) is pressed
- `Length`: Converts the counter into a string and prints it using stack-based digit printing logic

---

## 💬 Sample Output
![image](https://github.com/user-attachments/assets/8096c7a4-293b-4374-b9b1-24c16d9bb485)





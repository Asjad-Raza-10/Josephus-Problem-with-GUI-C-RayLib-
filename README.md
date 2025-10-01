# Josephus Problem with GUI (C++ & RayLib)

This project is a **visualization of the Josephus Problem** implemented in **C++** using the [RayLib](https://www.raylib.com/) graphics library.  
It provides an **interactive GUI** where users can input the number of people (`n`) and the elimination step (`k`), then watch the elimination process unfold step by step.

---

## 📌 Problem Intuition
The **Josephus Problem** is a famous theoretical problem:
- People stand in a circle and count off.
- Every `k`-th person is eliminated.
- The process continues until only one person remains.
- The challenge is to determine the position of the survivor.

This project turns that abstract problem into a **visual and interactive experience**.

---

## ⚙️ Logic Behind the Code
- A **circular doubly linked list** (`CircularQueue`) is implemented to represent the people standing in a circle.
- Each elimination is performed by moving forward `k - 1` steps and removing that person from the circle.
- The program supports:
  - **Loading `n` people** into the circle.
  - **Step-by-step elimination** on pressing `Enter`.
  - **Restart option** to try different values of `n` and `k`.

---

## 🎮 Features
- Interactive **GUI-based visualization** of the Josephus Problem.
- User inputs:
  - **Number of People (n)**  
  - **Elimination Count (k)**
- Each elimination is **highlighted in real-time**.
- Final **winner is shown clearly**.
- Option to restart with new values.

---

## 🚀 How to Run
Make sure you have **RayLib** installed. On MacBook, you can run the project with:

```bash
g++ -std=c++17 your_code.cpp -o executable_file -I/opt/homebrew/include -L/opt/homebrew/lib -lraylib -framework OpenGL -framework Cocoa -framework IOKit -framework CoreVideo
./executable_file

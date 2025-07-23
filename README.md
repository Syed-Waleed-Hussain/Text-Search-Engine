# 🔍 Text Search Engine using SFML (C Language - Theory of Automata Project)

This is a GUI-based Text Search Engine implemented in **C language style** with **SFML (Simple and Fast Multimedia Library)** for graphical display. It is designed as a practical project for the **Theory of Automata** course, simulating regular expression parsing using finite automata concepts.

---

## 📘 Project Objective

The program allows users to:
- Enter a regular expression
- Search for matching words from a text file
- Replace matched words (single or all)
- Display text content in a GUI window
- Learn how regex works internally through recursion and string parsing

---

## 💡 Features

- ✅ **Find**: Locate the first word matching the given RE
- ✅ **Find All**: List all matches in `words.txt`
- ✅ **Replace**: Replace the first matched word with another
- ✅ **Replace All**: Replace all matched words
- ✅ **View File**: Graphically view the contents of the file
- 🖼️ **SFML Interface**: Windowed interface with font and image background

---

## 🧠 Regular Expression Rules Supported

| Pattern      | Meaning                              |
|--------------|--------------------------------------|
| `a`          | Matches character `a`                |
| `a*`         | Matches 0 or more `a`s               |
| `a+`         | Matches 1 or more `a`s               |
| `(ab)+`      | Matches 1 or more of "ab"            |
| `(a|b|c)`    | OR between characters (up to 6)      |

---

## 🗂️ File Descriptions

| File Name    | Description                              |
|--------------|------------------------------------------|
| `main.c`     | Core logic and UI                        |
| `file.txt`   | The file from which words are searched   |
| `words.txt`  | Output file where matches are written    |
| `temp.txt`   | Temporary file for replacements          |
| `arial.ttf`  | Font used in SFML                        |
| `15.jpg`     | Background image                         |

---

## ⚙️ Compilation & Execution

### 💻 Linux / WSL Setup

```bash
sudo apt install libsfml-dev
gcc main.c -o TextSearchEngine -lsfml-graphics -lsfml-window -lsfml-system
./TextSearchEngine
# 🔍 Text Search Engine using SFML – Theory of Automata Project

This is a GUI-based **Text Search Engine** developed using **C/C++ and SFML (Simple and Fast Multimedia Library)**. It implements basic **regular expression matching** and file manipulation functionalities through a visually interactive interface.
```
---

## ⚙️ Compilation & Note

> **Note:** If `main.c` contains any C++ code, **rename it to `main.cpp`** and compile using `g++` instead of `gcc`.

---

## 🪟 Windows Setup (MinGW or Visual Studio)

1. Download SFML from [https://www.sfml-dev.org](https://www.sfml-dev.org)
2. Link SFML in your IDE’s project settings
3. Place `arial.ttf` and `15.jpg` in the same directory as your compiled executable

---

## 🧪 How It Works

- **Regex Matching** is performed using a recursive function:  
  `bool match(word, regex)`
  
- **String Parsing** uses basic C/C++ methods:  
  `fopen`, `fgets`, `strcpy`, `strcmp`, etc.

- **Graphics** are handled using **SFML** for:
  - Rendering text
  - Displaying buttons
  - Setting background visuals

---

## 📌 Sample Use Case

1. **User Input:** `(ab)*c`
2. **Program Action:**
   - Reads content from `file.txt`
   - Extracts words and matches them against the regex
   - Writes results to `words.txt`
3. **User Option:**
   - Selects `Replace` or `Replace All` to update the file content accordingly

---

## 🧑‍💻 Author

**Syed Waleed Hussain**  
Computer Science Student – FAST NUCES  
Theory of Automata Project – Summer 2025

---

## 📄 License

This project is **academic** and **open-source for educational use only**.  
Feel free to use, adapt, and expand for learning or teaching purposes.

---

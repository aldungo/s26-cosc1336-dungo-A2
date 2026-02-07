# Assignment 1: Personal Information Display

Welcome! This assignment will help you practice basic output in C++ using the `cout` statement.

## What You'll Learn
- How to use `cout` to display text
- How to use escape sequences like `\n` for new lines
- How to format output across multiple lines with a single statement

## Assignment Requirements

Write a C++ program that displays your personal information. Display the following, **each on a separate line**:

1. Your name
2. Your address (street address)
3. Your city, state, and ZIP code
4. Your telephone number
5. Your college major

### ⚠️ Important Rule

**Use only ONE `cout` statement** to display all of this information.

## Example Output

Your program should produce output like this (with your actual information):

```
John Doe
456 Oak Avenue
San Antonio, TX 78209
(210) 555-9876
Computer Science
```

---

## Step-by-Step Instructions

### Step 1: Open the Terminal

In GitHub Codespaces, you should see a terminal at the bottom of your screen. If you don't see it, you can open one by:
- Clicking on the menu: **Terminal → New Terminal**

### Step 2: Verify You're in the Right Directory

Make sure you're in the project directory by running:

```bash
pwd
```

You should see a path that indicates you're in your assignment repository.

### Step 3: Edit Your Code

1. Open the `a1main.cpp` file in the editor
2. Find the TODO comment
3. Replace the placeholder text with your actual information
4. Remember: Use **only ONE `cout` statement**!

### Step 4: Compile the Program

To compile your program, type the following command in the terminal:

```bash
g++ a1main.cpp -o a1main
```

**What this does:**
- `g++` - This is the C++ compiler
- `a1main.cpp` - This is the source file we want to compile
- `-o a1main` - This tells the compiler to create an executable file named `a1main`

If the compilation is successful, you won't see any output. No news is good news!

### Step 5: Run the Program

Now that you've compiled the program, run it with:

```bash
./a1main
```

**What this does:**
- `./a1main` - This runs the executable file we just created

### Step 6: Verify Your Output

Check that your output displays all five pieces of information, each on a separate line.

If it looks correct, congratulations! 🎉

---

## Troubleshooting

**If you get a "command not found" error:**
- Make sure you typed the command exactly as shown
- Make sure you completed Step 4 (compilation) before Step 5 (running)

**If you get compilation errors:**
- Check for missing semicolons (`;`)
- Check for mismatched quotes (`"`)
- Make sure you have `#include <iostream>` at the top
- Make sure you have `using namespace std;`

**If your output is all on one line:**
- Make sure you're using `\n` to create new lines
- Example: `cout << "Line 1\n" << "Line 2\n";`

---

## Understanding Escape Sequences

To display multiple lines with one `cout` statement, use `\n` (newline):

```cpp
cout << "Your Name\n"
     << "Your Address\n"
     << "Your City, State, ZIP\n"
     << "Your Phone\n"
     << "Your Major\n";
```

**Common escape sequences:**
- `\n` = new line (moves to the next line)
- `\t` = tab (adds spacing)
- `\"` = displays a quotation mark

---

## Design Document

After you complete your program, answer these questions below:

### What does your program do?
[Replace this with 1-2 sentences describing your program]

### What was challenging?
[Replace this with what you found difficult or what you learned]

### How did you test it?
[Replace this with how you verified your program works correctly]

---

## Submission to Canvas

1. **Download `a1main.cpp`** from your Codespace:
   - Right-click the file → Download
2. **Take screenshots** showing:
   - Your compilation command and result
   - Your program running with the correct output
3. **Upload to Canvas:**
   - Your `a1main.cpp` file
   - Your screenshots

**Note:** This README with your design document answers stays in GitHub - don't upload it to Canvas.

---

## Next Steps
- Try adding more information to your output
- Experiment with `\t` to add tabs
- Add decorative lines using special characters

Good luck! 🚀

# Assignment 2: Pizza Slice Calculator

Welcome! This assignment will help you practice working with variables, constants, calculations, and formatted output in C++.

## What You'll Learn
- How to declare and use named constants
- How to perform mathematical calculations
- How to use `cin` to get user input
- How to format output with `fixed` and `setprecision`
- How to work with the `<iomanip>` library

## Assignment Requirements

**Joe's Pizza Palace** needs a program to calculate the number of slices a pizza of any size can be divided into. Your program should:

1. Ask the user for the diameter of the pizza in inches
2. Calculate the number of slices that may be taken from a pizza of that size
3. Display a message telling the number of slices

### Key Facts

To calculate the number of slices, you need to know:

- **Each slice should have an area of 14.125 square inches**
- **Pizza area formula:** `Area = π × r²`
  - Use **3.14159** for π (pi)
  - `r` is the radius of the pizza
  - To get the radius, divide the diameter by 2
- **Number of slices:** Divide the pizza area by 14.125

### ⚠️ Important Requirements

- Use a **named constant** for PI
- Display the number of slices in **fixed-point notation**
- Round the output to **one decimal place**

## Example Output

Your program should produce output like this:

```
Enter the diameter of the pizza in inches: 16
A 16 inch pizza can be divided into 14.2 slices.
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

1. Open the `a2main_skeleton.cpp` file in the editor (or create `a2main.cpp` from scratch)
2. Find the TODO comments
3. Complete each section:
   - Declare constants (PI and SLICE_AREA)
   - Declare variables (diameter, radius, pizzaArea, numberOfSlices)
   - Get user input for diameter
   - Perform calculations (radius, area, slices)
   - Display formatted output

### Step 4: Compile the Program

To compile your program, type the following command in the terminal:

```bash
g++ a2main.cpp -o a2main
```

**What this does:**
- `g++` - This is the C++ compiler
- `a2main.cpp` - This is the source file we want to compile (rename from skeleton or create new)
- `-o a2main` - This tells the compiler to create an executable file named `a2main`

If the compilation is successful, you won't see any output. No news is good news!

### Step 5: Run the Program

Now that you've compiled the program, run it with:

```bash
./a2main
```

**What this does:**
- `./a2main` - This runs the executable file we just created

### Step 6: Test Your Program

Test with different pizza sizes:
- Try a 12-inch pizza (should give approximately 8.0 slices)
- Try a 16-inch pizza (should give approximately 14.2 slices)
- Try a 20-inch pizza (should give approximately 22.3 slices)

Make sure your output shows exactly **one decimal place**.

If it looks correct, congratulations! 🎉

---

## Troubleshooting

**If you get a "command not found" error:**
- Make sure you typed the command exactly as shown
- Make sure you completed Step 4 (compilation) before Step 5 (running)

**If you get compilation errors:**
- Check for missing semicolons (`;`)
- Make sure you have `#include <iostream>` at the top
- Make sure you have `#include <iomanip>` (needed for `fixed` and `setprecision`)
- Make sure you have `using namespace std;`
- Check that all variables are declared with their types (e.g., `double diameter;`)

**If your output doesn't show one decimal place:**
- Make sure you use `fixed` and `setprecision(1)` before displaying the number
- Example: `cout << fixed << setprecision(1) << numberOfSlices;`

---

## Understanding Named Constants

A **named constant** is a variable whose value cannot be changed after it's declared. Use the `const` keyword:

```cpp
const double PI = 3.14159;
const double SLICE_AREA = 14.125;
```

**Benefits of constants:**
- Makes code more readable
- Prevents accidental changes to important values
- Easy to update if the value needs to change later

## Understanding Formatted Output

To format decimal output, use `<iomanip>` library functions:

```cpp
#include <iomanip>

cout << fixed << setprecision(1);  // Show 1 decimal place
cout << numberOfSlices;             // This will display with 1 decimal
```

**Formatting options:**
- `fixed` = use fixed-point notation (not scientific notation)
- `setprecision(1)` = show 1 digit after the decimal point
- These settings apply to all following output until changed

---

## Design Document

After you complete your program, **answer the design document questions in the comments at the top of your `a2main.cpp` file**. You'll find a section that looks like this:

```cpp
/*
===========================================
DESIGN DOCUMENT
===========================================

What does your program do?
[Replace this with 1-2 sentences describing your program]

What was challenging?
[Replace this with what you found difficult or what you learned]

How did you test it?
[Replace this with how you verified your program works correctly]

===========================================
*/
```

Replace the placeholder text with your answers directly in the .cpp file.

---

## Submission to Canvas

### Step 1: Complete Your Design Document
Make sure you've filled out the design document questions in the comments at the top of your `a2main.cpp` file.

### Step 2: Download Your File from Codespaces

**Method 1: Right-click Download**
1. In the file explorer on the left, find `a2main.cpp`
2. Right-click on the file
3. Select **"Download"**
4. The file will be saved to your computer's Downloads folder

**Method 2: File Menu Download**
1. Open `a2main.cpp` in the editor
2. Click **File** → **Download**
3. The file will be saved to your Downloads folder

### Step 3: Take Screenshots

Capture screenshots showing:
1. **Compilation:** Your terminal with the `g++` command and successful compilation
2. **Test Run 1:** Your program running with a 12-inch pizza
3. **Test Run 2:** Your program running with a 16-inch pizza

**How to take screenshots:**
- **Windows:** Press `Windows Key + Shift + S` to use Snipping Tool
- **Mac:** Press `Cmd + Shift + 4` to capture a selection
- **Linux:** Press `PrtScn` or use screenshot tool

### Step 4: Upload to Canvas

1. Go to your Canvas assignment page
2. Click **"Submit Assignment"**
3. Upload the following files:
   - ✅ `a2main.cpp` (downloaded from Codespaces)
   - ✅ Your compilation screenshot
   - ✅ Your test run screenshots
4. Click **"Submit"**

**Important:** Make sure your `a2main.cpp` includes:
- ✅ Your completed code
- ✅ Your design document answers in the comments
- ✅ Proper formatting (fixed-point with 1 decimal place)

**Note:** You do NOT need to upload the README.md file to Canvas.

---

## Next Steps
- Try calculating the cost per slice if you know the pizza price
- Modify the program to calculate how many pizzas are needed for a party
- Experiment with different slice sizes

Good luck! 🍕

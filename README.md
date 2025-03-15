# Spreadsheet-with-JS

You can access the full project here:
https://fadliazharr.github.io/Spreadsheet-with-JS/

## Overview  

This project is a **functional programming-based spreadsheet application** built using **HTML, CSS, and JavaScript**. It allows users to input formulas similar to those in Excel or Google Sheets, perform calculations, and manipulate data dynamically.  

## Features  

- Supports basic arithmetic operations (`+`, `-`, `*`, `/`).  
- Implements spreadsheet functions like `sum`, `average`, `median`, and more.  
- Supports **cell references** (e.g., `=A1+B2`).  
- Allows users to define number ranges (`A1:A5`) and apply functions to them.  
- Uses **pure functions** for calculations, ensuring predictable results.  

## How It Works  

### 1. Grid Setup  
- The spreadsheet consists of a **grid layout** generated dynamically using JavaScript.  
- Columns are labeled **A–J**, and rows are numbered **1–99**.  
- Each cell is an `<input>` field where users can enter data or formulas.  

### 2. Formula Parsing & Evaluation  
- When a user enters a formula (e.g., `=A1+A2`), the program:  
  1. **Extracts cell references** and replaces them with their values.  
  2. **Processes mathematical operations** using predefined functions.  
  3. **Expands functions** like `sum(A1:A3)`, replacing the range with actual values.  
  4. **Evaluates the final expression** and updates the cell with the result.  

### 3. Functional Approach  
- The spreadsheet relies on **pure functions** to avoid side effects.  
- Functions like `sum`, `average`, and `median` process arrays and return results without modifying global state.  
- Uses **higher-order functions** for operations like filtering even numbers or removing duplicates.  

## How to Use  

1. Open the `index.html` file in a web browser.  
2. Click on any cell and enter:  
   - **A number** → Direct input.  
   - **A formula** → Start with `=` (e.g., `=A1+A2` or `=sum(A1:A5)`).  
3. Press **Enter** to evaluate the formula.  

## Example Inputs & Outputs  

| Input | Expected Output | Description |
|--------|---------------|-------------|
| `=5+3` | `8` | Basic arithmetic |
| `=A1*A2` | `Product of A1 and A2` | Cell reference multiplication |
| `=sum(A1:A3)` | `Sum of values in A1 to A3` | Range-based function |
| `=median(A1:A5)` | `Middle value of A1 to A5` | Statistical function |

## Technologies Used  

- **HTML** → Defines the structure of the spreadsheet.  
- **CSS** → Styles the grid and labels.  
- **JavaScript** → Handles calculations, formula parsing, and DOM manipulation.  

## Future Improvements  

- Add support for more **spreadsheet functions** (e.g., `IF`, `VLOOKUP`).  
- Implement **persistent storage** to save user data.  
- Improve **UI/UX** with better styling and usability.  

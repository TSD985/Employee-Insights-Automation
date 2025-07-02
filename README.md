### 📊 Employee Data Processor – UiPath Mini Project

This project demonstrates how UiPath can automate and process structured Excel-based employee data. The workflow handles filtering, counting, and reporting using key UiPath activities and logical structures.

--- 

### 📝 Project Overview

The workflow processes an Excel file containing employee details and performs the following tasks:

### Key Tasks & Features

#### 1. Filter Employees by Experience :
- Objective: Extract employees with more than 3 years of experience.
- Output: Stored in a new sheet called `Experienced Employees`
- Activities Used:
  - Read Range
  - Filter Data Table
  - Write Range

#### 2. Count Employees in Each Department :
- Objective: Count the number of employees in departments like HR, IT, Finance, and Sales.
- Output: Written to a new sheet called `Department Summary`
- Logic:
  - Used If conditions inside a For Each Row
  - Maintained counters like countHR, countIT, etc.
  - Used Build Data Table and Add Data Row to summarize

#### 3. Get All Sheet Names :
- Objective: Dynamically list all sheet names in the Excel workbook.
- Activity Used: Get Workbook Sheets

#### 4. Filter Employees Joined in 2023 or Later :
- Objective: Identify employees who joined in 2023 or later.
- Logic:
  - Used DateTime.Parse(row("JoiningDate"))
  - Compared joining year with >= 2023
- Output: Logged employee names using Log Message

---

### Tech Stack
- Tool: UiPath Studio (Desktop)
- Input File: Excel Spreadsheet
- Key Activities:
  - Read Range, Filter Data Table, Write Range
  - Assign, If, For Each Row
  - Build Data Table, Add Data Row
  - Get Workbook Sheets
  - Log Message

---

### Use Cases
- Automating HR analytics and reporting
- Creating filtered views of employee data
- Department-level summaries
- Tracking recent hires dynamically
- Handling multi-sheet Excel automation

---

### Learning Outcomes
- Filter data using condition-based logic  
- Build and populate summary tables programmatically  
- Handle dates with DateTime.Parse()  
- Use counters for grouped data insights  
- Log filtered results for tracking  
- Write results to new Excel sheets dynamically

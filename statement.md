# Smart Finance Tracker - Project Documentation

## 1. Problem Statement
The core problem this project addresses is the need for a **simple, user-friendly, command-line based system** to track personal or small-scale financial transactions (income and expenses).  

Existing solutions are often overly complex (requiring external spreadsheets or dedicated software) or lack persistent storage. This application aims to provide a solution that allows users to:
- Quickly log transactions
- Categorize income/expenses
- Generate immediate summaries
- **Automatically save and reload** data via a standard CSV file (`finance_data.csv`).
---

## 2. Scope of the Project

### Inclusions (What the project covers)
- **Data Persistence**:  
  Loading and saving transaction records to/from a local file named `finance_data.csv`.
- **Transaction Recording**:  
  Ability to input new transactions, clearly marking them as `income` or `expense`.
- **Data Fields**:  
  Recording `Type`, `Amount` (validated as numeric), `Category/Source`, and `Description`.
- **Basic Reporting**:  
  Generating an immediate summary view showing:
  - Total income
  - Total expense  
  - Net balance
  - Categorized breakdown of expenses.
- **Data Visualization (Terminal)**:  
  Use of **color-coding** (Green for income, Red for expense, Blue/Yellow for structure) to enhance terminal readability.
- **Export Functionality**:  
  Ability to export the financial summary into a structured CSV file (`summary_report.csv`).

### Exclusions (What is NOT covered in this version)
- **Graphical User Interface (GUI)**:  
  The application is strictly a **Command-Line Interface (CLI)**.
- **Advanced Data Manipulation**:  
  Features like editing, deleting, or searching existing transactions are **not included**.
- **Budgeting/Forecasting**:  
  The system reports **historical data only** – no future planning.
- **Database Integration**:  
  Data is stored in a simple CSV file, **not** a relational database (e.g., SQLite, MySQL).
- **Recurring Transactions**:  
  No mechanism to set up repeating/recurrent entries.

---

## 3. Target Users
The primary target users for this application are individuals who need a straightforward tool without complex software overhead:

- **Students**  
  Track allowances, part-time job earnings, and weekly spending (food, entertainment).
  
- **Freelancers/Gig Workers**  
  Log sporadic income and project-related expenses without formal accounting software.
  
- **Beginner Budgeters**  
  New users who want immediate categorization of spending habits.
  
- **Small Household Managers**  
  Track basic monthly household cash flow with simple persistent storage.

---

## 4. High-Level Features

The application is built around **four main functional areas**, accessible via the main menu:

| Feature Area              | Description                                                                 | Menu Options                          |
|---------------------------|-----------------------------------------------------------------------------|---------------------------------------|
| **Data Entry**            | Input structured financial data with validation for numeric amounts.        | `1` (Add Income), `2` (Add Expense)   |
| **Data Retrieval & Saving** | Automatically loads existing transactions on startup and saves all records on exit. | Automatic (No manual input required) |
| **Financial Reporting**   | Calculates and displays: <br> • Total income <br> • Total expenses <br> • Net balance <br> • Expense category breakdown (color-coded). | `3` (View Summary & Breakdown), `4` (View All Transactions) |
| **Data Export**           | Exports the summarized report to a new structured CSV (`summary_report.csv`). | `6` (Export Summary to New CSV)       |

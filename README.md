# 💰 Smart Finance Tracker (Python CLI)

A lightweight, interactive command-line application to help users track personal finances by recording income and expenses, viewing summaries, and analyzing spending patterns — all built with core Python concepts.

[![Python](https://img.shields.io/badge/Python-3.6%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🎯 Project Overview

This project serves as a practical implementation of fundamental programming concepts learned in an introductory course like **CSE1021: Introduction to Problem Solving and Programming**. It allows users to:

- Log income and expense transactions
- View real-time financial summaries
- Analyze spending by category with percentage breakdowns
- Persist data across sessions using JSON storage

The goal is to reinforce understanding of control structures, data types, functions, and file I/O while building a functional tool.

---

## ✨ Features

✅ **Add Income**  
Record sources of income (e.g., salary, freelance, gifts) with amount, source, and description.

✅ **Add Expense**  
Log expenses categorized by purpose (e.g., Food, Rent, Transport) for better organization.

✅ **View Summary & Breakdown**  
- Total Income  
- Total Expenses  
- Net Balance (color-coded: green for positive, red for negative)  
- **Categorical Expense Analysis**: See how much each category contributes to overall spending (in percentages).

✅ **View All Transactions**  
Display a neatly formatted, color-coded table of all recorded transactions with IDs, types, amounts, categories/sources, and descriptions.

✅ **Auto-Save on Exit**  
All data is automatically saved to `finance_data.json` when exiting, and reloaded on next startup.

✅ **User-Friendly CLI Interface**  
Clean menu navigation with input validation and colorful feedback using ANSI escape codes.

---

## 📦 Installation & Setup

### Prerequisites
- Python 3.6 or higher
- No external libraries required (uses only built-in modules: `json`)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/smart-finance-tracker.git
   cd smart-finance-tracker
  

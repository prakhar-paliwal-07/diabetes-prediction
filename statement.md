# Project Statement: Command-Line Finance Tracker

This document outlines the **core purpose**, **boundaries**, **intended audience**, and **main capabilities** of the Python-based Command-Line Finance Tracker application.

## Problem Statement

The lack of a simple, quick, and accessible tool for daily personal financial tracking can lead to poor budgeting, inadequate savings, and a generalized lack of awareness regarding personal spending habits. Existing sophisticated software is often overwhelming or requires complex setup.

**The goal** is to provide a minimalist, command-line application that allows a user to quickly record income and expenses and instantly view a net balance — encouraging consistent financial habit-tracking without the distraction of complex features.

## Scope of the Project

### In Scope (Current Project)

| Functionality          | Description                                                                                           |
|------------------------|-------------------------------------------------------------------------------------------------------|
| **Input**              | Accepting only four core data points for expenses (`Description`, `Amount`, `Category`, `Date`) and three for income (`Source`, `Amount`, `Date`) via the command line. |
| **Calculation**        | Generating three summary metrics: **Total Income**, **Total Expenses**, and **Net Balance** (Income − Expenses). |
| **Persistence**        | Saving and loading the entire dataset to a single local file (`finance_data.json`) to retain records between sessions. |
| **Interface**          | Operation exclusively through the **command-line interface (CLI)**.                                   |

### Out of Scope (Explicitly Excluded)

- Advanced query/filtering (e.g., finding all expenses in March)  
- Data visualization (charts, graphs)  
- Multi-user support or cloud synchronization  
- Editing or deletion of existing transactions  
- Advanced budgeting or goal-tracking features  

## Target Users

The application is designed for individuals who meet the following criteria:

- **Beginner Trackers** – Users who are just starting to monitor their finances and need a non-intimidating tool.  
- **CLI Users** – Individuals comfortable interacting with command-line applications (developers, students, or power users).  
- **Simple Budgeters** – Users who only require a quick, accurate overview of income versus spending.

## High-Level Features

| Feature Category      | Description                                                                                              |
|-----------------------|----------------------------------------------------------------------------------------------------------|
| **Transaction Entry** | Allows the user to quickly input new income and expense records using dedicated menu options.           |
| **Financial Summary** | Calculates and displays three immediate summary metrics: **Total Income**, **Total Expenses**, and **Net Balance**. |
| **Data Persistence**  | Automatically loads all previous records upon startup and saves the current state when the user selects **Exit**. |
| **Basic Error Handling** | Includes simple checks to ensure that the user inputs numerical values for the `Amount` fields.        |

---

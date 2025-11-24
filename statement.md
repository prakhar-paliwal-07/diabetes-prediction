# Project Statement: Command-Line Finance Tracker

This document explains the **main purpose**, **limits**, **target audience**, and **key features** of the Python-based Command-Line Finance Tracker application.


## Problem Statement

There is a lack of an easy, fast, and easy-to-use tool for daily personal financial tracking, which can result in poor budgeting, insufficient savings, and a general unawareness of spending habits.
 Many existing tools are too complex or require a lot of setup.

**The goal** is to create a simple, command-line application that lets users easily record income and expenses and instantly see their net balance, promoting consistent financial tracking without the distraction of complicated features.


## Scope of the Project

### Included in the Project

| Functionality | Description |
|------------------------|-------------------------------------------------------------------------------------------------------|
| **Input** | Accepting only four key pieces of information for expenses (`Description`, `Amount`, `Category`, `Date`) and three for income (`Source`, `Amount`, `Date`) via the command line.
 |
| **Calculation** | Calculating three summary values: **Total Income**, **Total Expenses**, and **Net Balance** (Income − Expenses).
 |
| **Persistence** | Saving and loading all data to a single local file named `finance_data.
json` to keep records between sessions. |
| **Interface** | Using the **command-line interface (CLI)** strictly for all operations.
 |

### Not Included in the Project

- Advanced search or filtering (e.g., finding all expenses in March) 
- Visual representations like charts or graphs 
- Support for multiple users or syncing with the cloud 
- Editing or deleting existing transactions 
- Budgeting or goal-tracking tools 

## Target Users

The application is intended for users who meet the following conditions:

- **Beginner Trackers** – Individuals who are new to tracking their finances and need an approachable tool.

- **CLI Users** – People who are comfortable using command-line applications (such as developers, students, or advanced users).

- **Simple Budgeters** – Users who only want a quick and accurate view of income versus expenses.


## High-Level Features

| Feature Category | Description |
|-----------------------|----------------------------------------------------------------------------------------------------------|
| **Transaction Entry** | Lets the user enter new income and expense records quickly through specific menu options.
 |
| **Financial Summary** | Displays three key summary values: **Total Income**, **Total Expenses**, and **Net Balance** immediately.
 |
| **Data Persistence** | Loads all previous records when the app starts and saves the current state when the user selects **Exit**.
 |
| **Basic Error Handling** | Has simple checks to ensure users enter numerical values for the `Amount` fields.
 |

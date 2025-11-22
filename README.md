# AKSHADA-SULE
Manage budget and daily expenses
# Smart Expense Tracker
 Project Title

Smart Expense Tracker (Console Version)

# Overview of the Project

This is a simple Python-based console application that helps users track their daily expenses and compare them with their monthly budget.
The program allows users to add expenses, view summaries, and get automated suggestions based on their spending habits.
All expenses are stored in a text file so that the user’s data remains saved even after closing the program.

 # Features

Add expenses with amount and notes

Automatically log date and time of each entry

Stores all expenses in a text file (expenses.txt)

Displays:

Total spent

Remaining budget

Category-wise spending summary (with bar chart visualization)

Gives smart suggestions based on spending behaviour

Simple menu-driven interface

 Technologies / Tools Used

# Python 3

Datetime module (for timestamping expenses)

File handling (reading & writing from a text file)

Console-based UI

# Steps to Install & Run the Project

Make sure Python 3 is installed on your system.

Download or copy the project code into a .py file (e.g., expense_tracker.py).

Ensure the script is in the same folder where you want expenses.txt to be created.

Open a terminal/command prompt.

Run the script:

python expense_tracker.py


Enter your monthly budget.

Choose actions from the menu to add or view expenses.

# Instructions for Testing

Start the program and enter any test budget (e.g., ₹10000).

Add multiple expenses using option 1.

Enter amounts like 200, 500, 1000 etc.

Add any short note.

Use option 2 to view:

Total spending

Remaining budget

# Flow chart of the program
┌────────────────────────┐
                   │      Start Program     │
                   └────────────┬───────────┘
                                │
                                ▼
                   ┌────────────────────────┐
                   │ Ask user for monthly   │
                   │        budget          │
                   └────────────┬───────────┘
                                │
                                ▼
                   ┌────────────────────────┐
                   │   Display Main Menu:   │
                   │ 1. Add Expense         │
                   │ 2. View Summary        │
                   │ 3. Exit                │
                   └────────────┬───────────┘
                                │
                      ┌─────────┼─────────┐
                      │         │         │
                      ▼         ▼         ▼

         ┌────────────────┐   ┌──────────────────┐   ┌────────────────────┐
         │ 1. Add Expense │   │ 2. View Summary  │   │ 3. Exit Program    │
         └───────┬────────┘   └──────────┬──────┘   └──────────┬─────────┘
                 │                       │                     │
                 ▼                       ▼                     ▼

    ┌──────────────────────┐   ┌───────────────────────┐   ┌────────────────────────┐
    │ Ask amount spent     │   │ Read all expenses      │   │ Display exit message   │
    │ Ask note             │   │ from expenses.txt       │   └────────────────────────┘
    │ Get current time     │   └──────────┬─────────────┘
    └──────────┬───────────┘              │
               │                           ▼
               ▼               ┌──────────────────────────┐
    ┌──────────────────────┐   │ Calculate total expenses │
    │ Write expense data    │   │ Calculate remaining     │
    │ into expenses.txt     │   │ budget                  │
    └──────────┬───────────┘   └──────────┬──────────────┘
               │                           │
               ▼                           ▼
   ┌────────────────────────┐   ┌──────────────────────────────┐
   │ Print success message  │   │ Show category-wise spending   │
   └──────────┬────────────┘   │ Generate bar chart             │
               │                └──────────┬─────────────────────┘
               │                           │
               ▼                           ▼
       ┌────────────────┐      ┌──────────────────────────────┐
       │ Return to Menu │◄──── │ Show suggestions              │
       └────────────────┘      └──────────┬─────────────────────┘
                                           │
                                           ▼
                                 ┌───────────────────┐
                                 │ Return to Menu    │
                                 └───────────────────┘

# ATM Simulator

A Python and MySQL desktop ATM simulation developed as a university team project. It explores object-oriented design, relational database operations, Tkinter interfaces, and threaded ATM sessions.

## Overview

The project models a small banking environment with banks, ATM terminals, customer accounts, cards, administrators, and transaction records. The Python classes interact with a MySQL/MariaDB database, while Tkinter provides a basic desktop navigation interface.

> **Project status:** This is an academic prototype, not production banking software. The current `main.py` provides a basic GUI navigation shell; the domain classes contain the account, card, ATM, bank, administrator, and transaction operations.

## Features represented in the project

- Card/PIN validation through the `Card` class.
- Account balance operations for deposits and withdrawals.
- ATM and account transaction-history queries.
- MySQL persistence for accounts, cards, banks, ATMs, administrators, and transactions.
- Thread-based ATM/account classes and synchronization locks.
- A Tkinter desktop entry point with ATM and Admin navigation screens.
- SQL schema and sample records for local setup.

## Tech Stack

| Area | Technology |
| --- | --- |
| Language | Python |
| Desktop UI | Tkinter |
| Database | MySQL / MariaDB |
| Database driver | mysql-connector-python |
| Concurrency concepts | threading, threading.Lock |
| Database script | SQL |

## Project Structure

```text
.
├── main.py              # Tkinter navigation shell
├── legacy_demo.py       # Preserved command-line demonstration workflow
├── ATM.py               # ATM operations and transaction logging
├── account.py           # Account model and balance operations
├── admin.py             # Administrator operations
├── bank.py              # Bank and ATM/account management
├── card.py              # Card validation and linked account
├── db.py                # MySQL connection and query helpers
├── login.py             # Administrator login
├── register.py          # Administrator registration
├── transaction.py       # Transaction model and history queries
├── atmsimulator.sql     # Database schema and demo records
└── requirements.txt     # Python package dependencies
```

## Setup

### 1. Prerequisites

- Python 3.9 or later
- MySQL Server or MariaDB
- A database client such as MySQL Workbench or phpMyAdmin

### 2. Clone the repository

```bash
git clone https://github.com/MernaAyman-l/ATM-Simulator-Python-MySQL.git
cd ATM-Simulator-Python-MySQL
```

### 3. Install Python dependencies

```bash
python -m venv .venv
```

Activate the environment:

**Windows PowerShell**
```powershell
.venv\\Scripts\\Activate.ps1
```

**macOS / Linux**
```bash
source .venv/bin/activate
```

Install the required package:

```bash
python -m pip install -r requirements.txt
```

### 4. Create the database

1. Start MySQL or MariaDB.
2. Create a database named `atmsimulator`.
3. Import `atmsimulator.sql` into that database.

The current database helper in `db.py` uses local defaults (`localhost`, user `root`, empty password). Update those settings in `db.py` to match your local MySQL configuration before connecting.

### 5. Run the current GUI shell

```bash
python main.py
```

The current entry point opens the Tkinter navigation shell. The ATM/Admin screens are starter interfaces; the backend classes and database operations are separate project components.

## My Contribution

- Served as the **Team Leader**.
- Worked on the **Tkinter graphical user interface**.
- Contributed to system design, including the **Sequence Diagram**.

## Team

- Merna Ayman Louis Soares — Team Leader
- Yara Ahmed Fathy Habib
- Adel Ali Ibrahim Ali
- Mahmoud Mohamed Ahmed Sayed
- Basma Mohamed Abdel Mouty Shehata
- Heba Adel Ali Abdel Khalik

**Instructor:** Dr. Ahmed Hesham

## Important Security Notes

This repository is an educational simulation only. The supplied SQL dump contains demonstration records, including simple sample PINs and administrator passwords, and the current code compares/stores credentials in plain text. Do not reuse those credentials or deploy this project with real banking or personal data. A production implementation would require password/PIN hashing, secure configuration through environment variables, input validation, transaction-safe database operations, and stronger authorization controls.

## Learning Goals

- Practice object-oriented programming in Python.
- Work with relational database schemas and SQL queries.
- Understand threads and synchronization concepts.
- Connect a desktop application to a MySQL/MariaDB database.
- Model basic ATM and banking workflows.

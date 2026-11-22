# 🏧 ATM Simulator

A Python-based ATM Simulation System that models concurrent banking operations using multithreading, synchronization locks, a Tkinter GUI, and a MySQL database.

## 📌 Project Overview

**ATM Simulator** is a desktop application that simulates multiple ATM sessions operating on shared banking records—including accounts, linked cards, banks, and transactions—while handling concurrent updates safely.

The system uses Python threads and synchronization locks to maintain balance consistency, log transactions, and generate PDF transaction history reports with visual plots.

## ✨ Key Features

- **User Authentication:** Validates card numbers and PINs before granting access to ATM services.
- **Deposit & Withdrawal:** Supports deposits and withdrawals with balance validation.
- **Balance Inquiry:** Displays and refreshes the current account balance.
- **Multithreading:** Handles multiple ATM sessions and operations concurrently.
- **Synchronization:** Uses locks (`threading.Lock`) to protect shared account balances from race conditions.
- **Transaction Logging:** Records transaction type, amount, timestamp, account ID, and ATM ID in MySQL.
- **PDF Report & Chart Generation:** Exports transaction history into a PDF report with a transaction amount plot.
- **Graphical User Interface:** Desktop interface built with Tkinter and Pillow (`PIL`).

## 🛠️ Technologies Used

- **Python:** Core application logic and object-oriented structure.
- **Tkinter & Pillow (`PIL`):** Desktop GUI development and image handling.
- **MySQL (`mysql-connector`):** Relational database for accounts, cards, banks, ATMs, admins, and transactions.
- **Threading (`threading.Thread`, `threading.Lock`):** Concurrent transaction processing and synchronization.
- **ReportLab & Matplotlib:** PDF statement generation and transaction amount plotting.
- **Traceback & Messagebox:** Error handling, debugging, and user notifications.

## ⚙️ Concurrency: Multithreading vs. Sequential Processing

The project illustrates how concurrent execution differs from sequential processing:

- **Sequential Processing:** Transactions run one after another, which can increase waiting time.
- **Multithreading:** Multiple ATM sessions can run concurrently, reducing idle wait times.
- **Synchronization:** Locks coordinate access to shared account balance updates so concurrent operations stay consistent.

## 📐 System Design

The project documentation includes system design diagrams illustrating workflows and interactions:

- **Use Case Diagram**
- **Activity Diagram**
- **Sequence Diagram**

## 👩‍💻 My Contribution

- Served as **Team Leader** for the project team.
- Developed and worked on the **Graphical User Interface (GUI)** using **Tkinter**.
- Participated in system design, including the **Sequence Diagram**.

## 👥 Team Members

1. Merna Ayman Louis Soares *(Team Leader)*
2. Yara Ahmed Fathy Habib
3. Adel Ali Ibrahim Ali
4. Mahmoud Mohamed Ahmed Sayed
5. Basma Mohamed Abdel Mouty Shehata
6. Heba Adel Ali Abdel Khalik

**Instructor:** Dr. Ahmed Hesham

## 🎯 Project Objectives

- Understand multithreading and concurrent programming in Python.
- Apply synchronization mechanisms to protect shared resources.
- Simulate core banking and ATM operations backed by a relational database.
- Build desktop GUI applications and generate structured transaction reports.

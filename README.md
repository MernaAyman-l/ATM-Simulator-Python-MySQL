# 🏧 ATM Simulator

A Python-based ATM Simulation System designed to demonstrate concurrent transaction processing using multithreading.

## 📌 Project Overview

The ATM Simulator is a desktop application that simulates an ATM banking environment where multiple ATM sessions can operate concurrently.

The project focuses on handling banking transactions safely and efficiently using Python's threading mechanisms, while demonstrating synchronization techniques to maintain account balance consistency.

## ✨ Key Features

- **User Authentication:** PIN-based authentication before accessing ATM services.
- **Deposit:** Add money to a user's account.
- **Withdrawal:** Withdraw money while checking available balance.
- **Balance Inquiry:** Display the current account balance.
- **Multithreading:** Handle multiple ATM sessions concurrently.
- **Synchronization:** Protect shared account data from race conditions.
- **Transaction Logging:** Record transaction details for tracking and auditing.
- **Graphical User Interface:** Interactive ATM interface built with Tkinter.

## 🛠️ Technologies Used

- **Python:** Core programming language.
- **Tkinter:** GUI development.
- **Threading:** Concurrent ATM transaction processing.
- **Pillow (PIL):** Image handling.
- **Traceback:** Error tracking and debugging.
- **Messagebox & Simpledialog:** User interaction and notifications.

## ⚙️ Concurrency: Multithreading vs. Sequential Processing

The project demonstrates the difference between sequential and concurrent transaction processing.

- **Sequential Processing:** Transactions are handled one at a time, which may increase waiting time.
- **Multithreading:** Multiple ATM sessions can process operations concurrently.
- **Synchronization:** Locks help prevent race conditions and ensure safe updates to shared account balances.

## 📐 System Design

The project includes system design diagrams to illustrate its structure and behavior:

- Use Case Diagram
- Activity Diagram
- Sequence Diagram

## 👥 Team Members

1. Merna Ayman Louis Soares
2. Yara Ahmed Fathy Habib
3. Adel Ali Ibrahim Ali
4. Mahmoud Mohamed Ahmed Sayed
5. Basma Mohamed Abdel Mouty Shehata
6. Heba Adel Ali Abdel Khalik

**Instructor:** Dr. Ahmed Hesham

## 🎯 Project Objectives

- Understand multithreading and concurrent programming.
- Apply synchronization mechanisms to shared resources.
- Simulate real-world ATM operations.
- Improve practical Python programming and GUI development skills.

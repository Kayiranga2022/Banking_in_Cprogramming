# Banking in C Programming 🏦

A simple console-based Bank Management System implemented in C. This mini-project demonstrates file handling, user interaction via the command line, and basic banking operations such as account creation, deposits, withdrawals, and transaction tracking.

---
## 📋 Features

- **Account Management**:  
  - Create new user accounts  
  - Delete existing accounts  
  - View account details

- **Transactions**:  
  - Deposit money  
  - Withdraw money  
  - View transaction history

- **Persistent Storage**:  
  - Uses plain text or binary files to store account and transaction data  
  - Data persists across multiple program runs

- **Modular C Code**:  
  - Separate files/functions for account operations, transactions, and file I/O  
  - Easy to maintain and extend

---
## 🛠️ Requirements

- A C compiler (e.g., `gcc` on Linux/Mac or `MinGW`/`TDM-GCC` on Windows)
- Standard C library (no external dependencies)

---
## 🚀 How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Kayiranga2022/Banking_in_Cprogramming.git
   cd Banking_in_Cprogramming
Compile the program (modify filenames as needed):

bash
Copy
Edit
gcc -o bank_management main.c accounts.c transactions.c fileio.c
Run it:

bash
Copy
Edit
./bank_management      # on Linux/Mac
bank_management.exe    # on Windows
Follow the menu prompts to create accounts, make deposits or withdrawals, and view results.

📌 Code Structure
bash
Copy
Edit
Banking_in_Cprogramming/
├── main.c              # Entry point; displays main menu
├── accounts.c/h        # User account creation, deletion, lookup utilities
├── transactions.c/h    # Handles deposits, withdrawals, transaction history
├── fileio.c/h          # Wraps file operations (reading/writing .txt or .dat files)
├── data/
│   ├── accounts.dat    # Stored account records
│   └── transactions.dat # Stored transaction logs
└── README.md
Note: Filenames may vary; adjust compilation commands accordingly.

🧩 Design & Architecture
Accounts and transactions are represented using C structs.

File I/O functions (fopen, fread, fwrite) manage data persistence.

The main flow uses a looped menu system to guide user actions until exit.

Modular separation helps isolate functionality (accounts, transactions, data layer).

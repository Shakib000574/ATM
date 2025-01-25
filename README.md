Virtual ATM System
Project Overview
This project simulates a Virtual ATM supporting Savings and Current accounts. It demonstrates key OOP concepts like Inheritance, Polymorphism, Encapsulation, and Abstraction. Operations include checking balance, depositing money, and withdrawing money, with overdraft support for Current Accounts.

Technologies Used
Programming Language: Java
Development Environment: Any Java IDE (e.g., IntelliJ IDEA, Eclipse) or command-line tools
Directory Structure
bash
Copy
Edit
VirtualATMSystem/
├── src/
│   ├── main/
│   │   ├── ATM.java               # Main entry point
│   │   ├── accounts/
│   │   │   ├── Account.java       # Base class for all account types
│   │   │   ├── SavingsAccount.java# Derived class for savings
│   │   │   └── CurrentAccount.java# Derived class for current
│   │   ├── services/
│   │   │   └── BankService.java   # Abstract class for services
├── README.md                      # Project description and instructions
How to Run
Command Line:

Navigate to the src/ directory.
Compile: javac main/ATM.java accounts/*.java services/*.java
Run: java main.ATM
IDE:

Import the project.
Set ATM.java as the main class.
Run the program.
OOP Concepts Demonstrated
Encapsulation: Sensitive data (e.g., balance) is hidden with private fields and accessed via public methods.
Inheritance: SavingsAccount and CurrentAccount inherit from Account, extending its functionality.
Polymorphism: withdraw() is overridden in both SavingsAccount and CurrentAccount to handle withdrawals differently.
Abstraction: BankService defines common operations (checkBalance, deposit, withdraw) for all account types.
Sample Output
vbnet
Copy
Edit
Welcome to the Virtual ATM!
1. Savings Account
2. Current Account
Select account type: 1
Menu: 
1. Check Balance
2. Deposit Money
3. Withdraw Money
4. Exit
Choose an option: 1
Balance: $1000.0
Choose an option: 2
Enter amount to deposit: 200
Successfully deposited $200.0
Choose an option: 3
Enter amount to withdraw: 300
Savings account withdrawal allowed: $300.0
Successfully withdrew $300.0
Choose an option: 4
Thank you for using the Virtual ATM!

License
This project is for educational purposes only and not for commercial use.


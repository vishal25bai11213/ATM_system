ATM Simulation System
A simple, beginner-friendly ATM simulation built with Python. This project demonstrates basic programming concepts like functions, dictionaries, loops, and user input handling.
About This Project
I built this ATM system as part of my Python learning journey. It's designed to be simple and easy to understand, using only basic Python concepts that you'd learn in your first few weeks of programming.
Features
    • Create Account: Register with a username and 4-digit PIN 
    • Login System: Secure login with username and PIN verification 
    • Check Balance: View your current account balance 
    • Deposit Money: Add money to your account 
    • Withdraw Money: Take money out (with balance checking) 
    • Transaction History: See all your deposits and withdrawals 
    • Logout: Safely logout from your account 
What I Learned
While building this project, I practiced:
    • Using functions to organize code 
    • Working with dictionaries to store data 
    • Using lists to track transactions 
    • Handling user input and validation 
    • Working with if/else statements and loops 
    • Basic error handling with try/except 
How to Run
    1. Make sure you have Python installed (Python 3.6 or higher) 
    2. Download the atm_system.py file 
    3. Open your terminal or command prompt 
    4. Navigate to the folder containing the file 
    5. Run the command: 
       python atm_system.py
How to Use
First Time Using the ATM
    1. Create an Account
        ◦ Choose option 2 from the main menu 
        ◦ Enter a username (can be anything you like) 
        ◦ Create a 4-digit PIN (only numbers, exactly 4 digits) 
        ◦ Enter an initial deposit amount (can be 0 or more) 
    2. Login
        ◦ Choose option 1 from the main menu 
        ◦ Enter your username 
        ◦ Enter your PIN 
Using the ATM Features
Once logged in, you can:
    • Check Balance: See how much money you have 
    • Deposit: Add money to your account 
    • Withdraw: Take money out (if you have enough balance) 
    • View History: See all your transactions 
    • Logout: Exit your account safely 
Example Usage
========================================
WELCOME TO ATM SIMULATION
========================================

========================================
WELCOME TO ATM SYSTEM
========================================
1. Login
2. Create Account
3. Exit
========================================
Enter choice: 2

--- CREATE ACCOUNT ---
Enter username: john
Enter 4-digit PIN: 1234
Enter initial deposit: $100
Account created successfully!
Your balance: $100.0

========================================
ATM MENU
========================================
1. Check Balance
2. Deposit Money
3. Withdraw Money
4. View Transaction History
5. Logout
========================================
Enter choice: 1

Your balance: $100.00
Project Structure
The project is organized into simple sections:
    • Global Variables: Store user data and current user 
    • Menu Functions: Display menus to the user 
    • Account Management: Create accounts and login 
    • Transaction Functions: Handle deposits, withdrawals, and history 
    • Main Program: Runs the entire ATM system 
Important Notes
⚠️ Data is NOT saved permanently - When you close the program, all accounts and transactions are lost. This is intentional to keep the project simple for beginners.
Things I Could Add Later
As I learn more Python, I'd like to add:
    • Save data to a file so it doesn't disappear 
    • Transfer money between accounts 
    • Add timestamps to transactions 
    • Improve error messages 
    • Add a transfer feature 
Requirements
    • Python 3.6 or higher 
    • No external libraries needed! 
Common Issues and Solutions
Problem: "Invalid choice!" message appears
    • Solution: Make sure you're entering numbers 1-5, not letters 
Problem: "PIN must be exactly 4 digits!"
    • Solution: Your PIN should only contain numbers and be exactly 4 digits long 
Problem: "Insufficient funds!"
    • Solution: You're trying to withdraw more money than you have. Check your balance first! 

What Makes This Project Special
This isn't a complex, production-ready banking system. It's a learning project that shows:
    • How to organize code with functions 
    • How to work with dictionaries and lists 
    • How to get user input and validate it 
    • How to build a simple menu-based program 
Perfect for beginners who are just learning Python!
License
This is a student project created for educational purposes. Feel free to use it, modify it, and learn from it!
Author
Created as part of my Python learning journey at VIT University.

Note: This is a simple educational project, not meant for real banking! It's designed to practice programming concepts in a fun, practical way.

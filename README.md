BankAccount Program
Overview
The BankAccount Java program simulates basic banking operations, allowing users to create accounts, deposit and withdraw funds, change addresses, and view account details. It maintains records of transactions and provides an interactive menu for account management.

Package
java
Copy code
package com.ace;
Class: BankAccount
The BankAccount class encapsulates the functionality for managing bank accounts. It includes operations for deposit, withdrawal, address change, and displaying account information.

Data Members
public static Scanner scr: Global Scanner object for user input.
static int id: Static integer for generating unique account IDs.
String uid: Unique account ID.
String name: Account holder's name.
String address: Account holder's address.
String type: Type of account (e.g., Savings, Checking).
double balance: Current account balance.
public static int no_of_trans: Static counter for tracking the number of transactions.
Constructors
Default Constructor: Initializes the account with null values.

java
Copy code
BankAccount() {
    uid = null;
    name = address = type = null;
}
Parameterized Constructor: Initializes the account with provided details and generates a unique ID.

java
Copy code
BankAccount(String name, String address, String type, double balance) {
    uid = UID();
    this.name = name;
    this.address = address;
    this.type = type;
    this.balance = balance;
}
Methods
UID: Generates a unique account ID.

java
Copy code
String UID() {
    return "BA" + Integer.toString(id++);
}
display(): Prints the account information.

java
Copy code
void display() {
    // Implementation
}
deposit(): Allows the user to deposit an amount into the account.

java
Copy code
void deposit() {
    // Implementation
}
withdraw(): Allows the user to withdraw an amount from the account.

java
Copy code
void withdraw() {
    // Implementation
}
changeAddress(): Updates the address of the account holder.

java
Copy code
void changeAddress() {
    // Implementation
}
Main Method
The main method provides a user interface to interact with the bank accounts. It supports the following operations:

Print account information.
Deposit money into an account.
Withdraw money from an account.
Change the address of an account holder.
Print the total number of transactions.
Exit the program.
Usage
Run the program.
Enter the number of depositors and their details.
Use the menu to perform operations on the accounts.
Example
plaintext
Copy code
Enter Numbers of depositors : 2
Enter Information for Depositor no. 1
Enter name : John Doe
Type of Account : Savings
Enter Address : 123 Elm St
Enter Balance : ₹5000

Enter Information for Depositor no. 2
Enter name : Jane Smith
Type of Account : Checking
Enter Address : 456 Oak St
Enter Balance : ₹3000

MENU FOR ACCOUNT MANIPULATION
1. Print information of any depositor
2. Add amount to the account of any depositor
3. Remove some amount from account of any depositor
4. Change Address of any depositor
5. Print total number of transactions
6. Exit the program...
Enter your Choice : 1
Depositor no. : 1
Notes
Ensure that the input provided is in the correct format to avoid runtime errors.
The program does not handle edge cases such as insufficient funds or invalid inputs.

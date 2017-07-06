This project is written in python language.For this i use python 3 and xampp server for database connectivity.
This code is written in eclipse using pydev and i run this code in command prompt.
Code is about the banking processes like deposit, withdrawal, transfer of funds and so on.
A bank typically has large number of customers and maintains the details of each customer i.e. what is the name of my customer, his address, account number, how much money is there in his account etc.
We also hear about multiple types of accounts like Saving account, Current account.
The project is to develop a banking application for a bank that has multiple customers spread across the country.
A customer can have either of the following type of accounts:
Savings Account – Generally used for temporary savings. Offers interest at the rate of 7.5% per annum on your savings. Maximum 10 withdrawals are allowed per month. No minimum balance is needed to open or maintain this account.
Current Account – Generally used by corporates and business men. No interest is offered on this account. No limit of on no. of withdrawals. A customer needs to have minimum 5K to open or maintain this account.
A customer can do following transactions:
Deposit and withdraw money in his account/s
Transfer money to other accounts
Print his account statement for given range of dates
Bank wants to maintain history of closed accounts i.e. which accounts have been closed on which dates. Bank admin can see this history.
Every customer has a customer-id and password to access his account.
When a new customer registers himself with the bank, a customer-id is auto generated by the bank and given to him.
Password needs to be set by the customer. It should be minimum 8 characters and can be any combination of numeric and alphabets.
Allow maximum 3 consecutive re-trials for unsuccessful login attempts.
Bank keeps following information of all customers to send regular updates
First and Last Name of customer
Address has following fields - Address Line 1, Line 2, City, State, Pincode. Pincode should be a 6 digit numeric and rest of the fields are strings.
Account no./s – Account no. is auto-generated by the bank on opening of a new account and is same as customer id.
Transactions (withdrawals & deposits) done by the customers on respective accounts
Interest on savings account is not getting applied.
Account once locked due to 3 successive erroneous password can not be unlocked.
Password is not encrypted.
Menu is like this:
  1.sign up
  2.sign in
  3.admin sign in
  4.quit
in sign un:
  propmt for new customer
   Add that customer based on necessary conditions (e.g. min balance). On successful creation of new customer, display auto-generated customer-id and account no. Prompt for a password and accept as per password rules. Display success or error messages as applicable.
in sign in:
  prompt for login and password
   Allow maximum 3 consecutive re-trials for unsuccessful login attempts. Display error messages as applicable.
Admin Sign In:
  Prompt for admin-id and password and validate. Allow 3 consecutive re-trials for successful login. Display success or error messages.   Admin id and password are fixed and stored in database.
Quit:
   Quit the application.
from main menu after successful login following menu:
A)Address Change:
  Prompt logged-in customer for new address and update as per entered address. Display success or error messages.
B)Money Deposit:
  Prompt logged-in customer for amount to be deposited and the account no. Validate (e.g. amount should not be negative, account no.      should be valid) and update. Display the new balance.
C)Money Withdrawal:
  Prompt logged-in customer for amount to be withdrawn and the account no. Validate (e.g. amount should be less than available balance,   min balance condition should be maintained based on account type, account no. should be valid) and update. Display the new balance.
  Write unit test cases as per Boundary conditions to test this use case.
D)Print Statement:
  Prompt logged-in customer for account no., “Date From” and “Date To”. Validate the entered values (e.g. Dates are valid, “Date To” is   greater than “Date From”, account no. should be valid), and display print statement with following values in a tabular format – Date,   Transaction Type (Credit, Debit), Amount, Balance
E)Transfer Money:
  Prompt logged-in customer for “Account To” and amount. Validate the entered values (e.g. “Account To” should be a valid account of any  customer, minimum balance in “Account From” should be maintained). Update both accounts and display new balances. The transaction should  be atomic i.e. if account balance is not updated properly in either “Account From” or “Account To”, entire transaction should be rolled  back.
F)Account Closure:
  Close the account so that no further operation like deposit, withdrawal is allowed on that account. Display the amount to be sent to  customer’s address after his account closure, and give successful closure message.
G)Customer Logout:
  Log out logged-in customer. Display successful logout message.
In admin login:
1.Print Closed Accounts History
  Display in a tabular format the list of closed account no.s with respective dates on which they were closed.
2.Admin Logout
  Log out admin. Display successful logout message.

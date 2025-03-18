I’ve created a Python-based Personal Expense Tracker that allows users to record, categorize, and monitor their expenses against a monthly budget. The application features a simple text-based menu interface and can save data to CSV files for future reference.
Core Features
1.	Adding Expenses: Users can add detailed expense records including date, category, amount, and description.
2.	Viewing Expenses: Displays all recorded expenses in a formatted table with a total.
3.	Budget Management: Users can set monthly budgets and track spending against these limits.
4.	Data Persistence: Expenses can be saved to and loaded from CSV files.
5.	User-Friendly Interface: A simple menu-driven interface for easy navigation.
Development Process
1. Planning and Design
I began by analyzing the requirements and planning the program's structure, breaking it down into five key components:
•	Data model for storing expenses and budget information
•	User input functions for adding expenses and setting budgets
•	Data processing functions for calculations and validations
•	File operations for saving and loading data
•	User interface for interaction
2. Implementation in Jupyter Notebook
I then implemented the application step-by-step in Jupyter Notebook, which allowed us to test each component individually:
1.	Setting Up the Environment: Imported necessary libraries and initialized global variables. 

2.	Core Functions: Created functions for each of the main features: 
o	add_expenses(): Collects and validates expense details
o	view_expenses(): Displays formatted expense records
o	set_budget(): Sets the monthly budget
o	track_budget(): Compares expenses against the budget
o	save_expenses(): Writes expenses to a CSV file
o	load_expenses(): Reads expenses from a CSV file

3.	User Interface: Implemented the menu system with show_menu() function to coordinate all operations.

4.	Program Execution: Created a main function to initialize and run the application.  You can run the application by calling main()
3. Debugging and Refinement
Throughout development, I addressed several issues:
•	Fixed naming inconsistencies between function names
•	Corrected date format validation to match the expected input
•	Ensured proper dictionary syntax with correct commas
•	Fixed variable name mismatches in the date validation logic
How the Application Works
1.	When started, the program attempts to load previously saved expenses.
2.	The main menu is displayed, offering seven options: 
o	Add Expense
o	View Expenses
o	Set Monthly Budget
o	Track Budget
o	Save Expenses
o	Load Expenses
o	Exit
3.	Each menu option calls the appropriate function: 
o	Adding an expense prompts for date, category, amount, and description with validation.
o	Viewing expenses displays all records with a total sum.
o	Setting a budget asks for a monthly limit.
o	Tracking the budget compares expenses against the set budget, showing remaining funds or warnings if exceeded.
o	Saving/loading handles file operations automatically.
4.	Before exiting, the program automatically saves data to preserve any changes.

![image](https://github.com/user-attachments/assets/035a96f9-0741-4610-bbb4-3390b2be7f23)

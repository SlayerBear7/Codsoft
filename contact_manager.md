Contact Management System
This is a simple command-line based Contact Management System implemented in Python. It allows users to store, view, search, update, and delete contact information.

Table of Contents
Features

How to Use

Code Explanation

Future Enhancements

License

Features
Add Contact: Store new contact details including store name, phone number, email, and address.

View Contact List: Display a numbered list of all saved contacts with their names and phone numbers.

Search Contact: Find contacts by searching for a store name or phone number (case-insensitive).

Update Contact: Modify existing contact details. Users can choose to update specific fields or keep existing ones.

Delete Contact: Remove unwanted contacts from the list.

User-Friendly Interface: Simple command-line menu for easy navigation.

Error Handling: Basic error handling for invalid user inputs (e.g., non-numeric choices).

How to Use
To run this Contact Management System:

Save the code: Save the provided Python code into a file named contact_manager.py (or any other .py extension).

Run from terminal: Open your terminal or command prompt, navigate to the directory where you saved the file, and run the script using Python:

python contact_manager.py

Follow the menu: Once the program starts, you will see a menu of options. Enter the number corresponding to the action you wish to perform and press Enter.

--- Contact Management System ---
1. Add Contact
2. View Contact List
3. Search Contact
4. Update Contact
5. Delete Contact
6. Exit
Enter your choice:

Code Explanation
The system is built around a ContactManager class that encapsulates all the contact management logic.

ContactManager Class:

__init__(): Initializes an empty list self.contacts to hold contact dictionaries.

add_contact(): Prompts for contact details and appends a new contact dictionary to self.contacts.

view_contact_list(): Iterates and prints a summary of all contacts.

search_contact(): Takes a search term, uses search_name_or_number helper, and displays matching contacts using display_contact_details.

update_contact(): Displays contacts, prompts for a contact to update, and allows modifying fields. Handles invalid input.

delete_contact(): Displays contacts, prompts for a contact to delete, removes it using pop(), and confirms deletion. Handles invalid input.

Helper Functions:

display_contact_details(contact): Prints all details of a given contact dictionary.

search_name_or_number(contact, search_term): Checks if the search_term is in the contact's name or phone number (case-insensitive).

main() Function:

Creates an instance of ContactManager.

Runs a while loop to display the main menu and handle user choices, calling the appropriate ContactManager methods.
In this project, I aimed to develop a simple yet effective book management application utilizing the "Shahre Ketab" database. This project incorporates the use of Jupyter Notebook for data exploration and manipulation, alongside a graphical user interface (GUI) built with Tkinter. The application includes several functions to handle various tasks efficiently, such as searching for books by their titles and inserting new books into the database.

The main components of the project include:

Database Connection: Establishing a connection to the "Shahre Ketab" SQL Server database using pyodbc to facilitate data retrieval and insertion.
Search Functionality: Implementing a search feature that allows users to query the database for books based on their titles. The results are displayed in a listbox within the Tkinter interface.
Insertion Functionality: Providing a form within the GUI for users to input new book details, including title, authors, ISBN, publisher, price, subject, and edition. The form data is then inserted into the database.
By integrating these elements, the application serves as a comprehensive tool for managing a collection of books, providing an intuitive interface for users to interact with the database.


Book Management Application
This is a simple Book Management Application developed using Python's Tkinter library for the GUI and pyodbc for connecting to a SQL Server database. The application allows users to search for books by name and insert new books into the database.

Features
Search Books: Search for books by their title.
Insert Books: Add new books to the database with details such as title, authors, ISBN, publisher, price, subject, and edition.
Requirements
Python 3.x
Tkinter (comes with Python)
pyodbc library
Installation
Clone the repository:

sh
Copy code
git clone https://github.com/iamalirezaebi/book-management-app.git
cd book-management-app
Install the required Python libraries:

You can use pip to install the pyodbc library if it is not already installed.

sh
Copy code
pip install pyodbc
Configure Database Connection:

Update the database configuration in the Python script as per your setup:

python
Copy code
server = 'localhost'
database = 'Shahre ketab'
username = 'YOUR_USERNAME'
password = 'YOUR_PASSWORD'
driver = '{ODBC Driver 17 for SQL Server}'
Usage
Run the application:

sh
Copy code
python book_management.py
Search for Books:

Enter the title of the book in the "Search Books" section.
Click the "Search" button to display the search results in the listbox.
Insert a New Book:

Fill in the details of the new book in the "Insert New Book" section.
Click the "Insert" button to add the book to the database.
Code Explanation
Database Connection:

The connect_to_db() function establishes a connection to the SQL Server database using the provided configuration.
Search Books:

The search_books() function retrieves books from the database whose titles match the search query and displays them in the listbox.
Insert Book:

The insert_book() function inserts a new book into the database with the details provided by the user.
Tkinter GUI:

The GUI is created using Tkinter. It has two main sections: one for searching books and another for inserting new books.

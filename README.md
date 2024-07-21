<!--
-- Author: Pavith Bambaravanage
-- URL: https://github.com/Pavith19
-->

![GitHub top language](https://img.shields.io/github/languages/top/Pavith19/Book-Management-System?style=flat)
![GitHub last commit](https://img.shields.io/github/last-commit/Pavith19/Book-Management-System?style=flat)
![ViewCount](https://views.whatilearened.today/views/github/Pavith19/Book-Management-System.svg?cache=remove)


# Book Management System

This is a simple Java-based application to manage a collection of books in a library. The application provides a console interface for adding, viewing, updating, deleting, and searching for books. It uses MySQL for storing book data.

## Features

- **Add a Book**: Add a new book to the database with a title, author, and publication year.
- **View All Books**: Display a list of all books in the database.
- **Update a Book**: Update the details of an existing book by its ID.
- **Delete a Book**: Remove a book from the database by its ID.
- **Search for a Book**: Search for books by title or author (case-insensitive).

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- MySQL Database
- MySQL Connector/J library

## Database Setup

1. Install MySQL and create a database named `library`.
2. Create a table named `books` with the following structure:

    ```sql
    CREATE TABLE books (
        id INT PRIMARY KEY,
        title VARCHAR(255) NOT NULL,
        author VARCHAR(255) NOT NULL,
        year INT NOT NULL
    );
    ```

3. Set the database connection credentials as environment variables:

    - **For Windows:**
      
      Temporarily (for the current Command Prompt session):
      
      ```cmd
      set DB_USER=root
      set DB_PASSWORD=your_password
      ```

      Permanently:

      - Open the **Start Menu** and search for "Environment Variables" and select "Edit the system environment variables."
      - Click on the **Environment Variables** button.
      - In the **User variables** section, click on **New...**.
      - Enter `DB_USER` as the variable name and `root` as the value.
      - Click **OK**.
      - Repeat the process for `DB_PASSWORD`, entering your MySQL password as the value.

    - **For macOS and Linux:**

      Temporarily (for the current terminal session):

      ```bash
      export DB_USER=root
      export DB_PASSWORD=your_password
      ```

      Permanently:

      - Open your terminal.
      - Edit your shell configuration file (`~/.bashrc`, `~/.bash_profile`, `~/.zshrc`, etc.), depending on the shell you are using. For example:

        ```bash
        nano ~/.bashrc
        ```

      - Add the following lines to the file:

        ```bash
        export DB_USER=root
        export DB_PASSWORD=your_password
        ```

      - Save the file and exit the editor.
      - Apply the changes by running:

        ```bash
        source ~/.bashrc
        ```

## How to Run

1. Clone the repository:

    ```bash
    git clone https://github.com/Pavith19/BookManagementSystem.git
    cd BookManagementSystem
    ```

2. Compile and run the application:

    ```bash
    javac -cp "path/to/mysql-connector-java.jar" BookManagementSystem.java
    java -cp ".;path/to/mysql-connector-java.jar" BookManagementSystem
    ```

    Replace `path/to/mysql-connector-java.jar` with the actual path to the MySQL Connector/J library on your system.

## Usage

- Run the application and follow the on-screen menu to manage the books in your library.
- Choose an option by entering the corresponding number and pressing Enter.

## Code Overview

The main methods in the `BookManagementSystem` class include:

- `addBook()`: Adds a new book to the database.
- `viewAllBooks()`: Displays all books in the database.
- `updateBook()`: Updates an existing book's details.
- `deleteBook()`: Deletes a book from the database.
- `searchBooks()`: Searches for books by title or author.
- `getYearInput()`: Gets a valid year input from the user.
- `getAvailableBookId()`: Gets the next available book ID.
- `printResults(ResultSet rs)`: Prints the results of a query.

## 🛠 Skills
MySQL, Java Programming & OOP

<h3 align="center">Connect with me:</h3>
<p align="center">
  <a href="https://instagram.com/_mr_2001__" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="_mr_2001__" height="30" width="40" /></a>
  <a href="https://linkedin.com/in/www.linkedin.com/in/pavith-bambaravanage-465300293" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="pavith-bambaravanage-465300293" height="25" width="35" /></a>
  <a href="https://www.hackerrank.com/@pavith_db" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/hackerrank.svg" alt="@pavith_db" height="40" width="45" /></a>
  <a href="https://www.leetcode.com/pavith_db" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" alt="pavith_db" height="30" width="40" /></a>
  <a href="mailto:pavithd2020@gmail.com" target="blank"><img align="center" src="https://github.com/TheDudeThatCode/TheDudeThatCode/raw/master/Assets/Gmail.svg" alt="pavithd2020@gmail.com" height="30" width="40" /></a>
</p>

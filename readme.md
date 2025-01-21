Library Management System

This is a console-based Library Management System implemented in C#. It demonstrates Object-Oriented Programming (OOP) concepts, adherence to SOLID principles, and the use of design patterns such as Singleton and Factory. The program allows users to add, remove, search, and list books and eBooks in a library.

Instructions to Run the Program

Set Up the Environment:

Install Visual Studio or any C# IDE.

Ensure the C# SDK is installed on your system.

Download and Extract:

Download the project ZIP file.

Extract it to a directory of your choice.

Open the Project:

Open Visual Studio.

Navigate to File > Open > Project/Solution.

Select the extracted folder and open the .csproj file.

Run the Program:

Set Program.cs as the startup file.

Build the solution (Ctrl + Shift + B) to ensure there are no compilation errors.

Run the program (F5 or click the green play button).

Interacting with the Program:

Use the text-based menu to add books or eBooks, remove books by ISBN, search for books by title, and list all books.

Key Features and Enhancements

Part 1: Basic Library Management System

Book Class:

Implements basic attributes: Title, Author, ISBN, and Available.

Includes a constructor for initializing attributes and a ToString method for formatted output.

Library Class:

Manages a collection of books using a list.

Provides methods to add, remove, search, and list books.

Part 2: Enhancements with OOP Principles

EBook Subclass:

Extends the Book class to include a FileSize attribute.

Overrides the ToString method to include file size information.

LibraryManager Class:

Introduces a menu-driven interface for interacting with the library.

Implements methods to handle user input and perform library operations.

Part 3: SOLID Principles and Design Patterns

Singleton Pattern:

Ensures only one instance of LibraryManager is created and accessed globally.

Factory Pattern:

Introduces BookFactory to handle the creation of Book or EBook objects based on user input.

Simplifies object instantiation and adheres to the Open/Closed Principle.

Application of SOLID Principles

Single Responsibility Principle (SRP):

Each class has a single responsibility:

Book and EBook: Represent book entities.

Library: Manages the collection of books.

LibraryManager: Handles user interactions.

BookFactory: Responsible for object creation.

Open/Closed Principle (OCP):

The Book class is open for extension (via EBook) but closed for modification.

Liskov Substitution Principle (LSP):

EBook objects can replace Book objects wherever Book is expected, without altering the program’s correctness.

Interface Segregation Principle (ISP):

Although not explicitly demonstrated, methods are kept specific and relevant to their respective classes.

Dependency Inversion Principle (DIP):

The LibraryManager relies on the abstraction (Library and BookFactory) rather than concrete implementations.

Design Patterns Used

Singleton Pattern:

Ensures a single instance of LibraryManager to manage user interactions globally.

Factory Pattern:

Encapsulates object creation logic, making it easier to manage and extend the system.

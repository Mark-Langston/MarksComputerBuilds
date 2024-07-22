# Mark's Computer Build

## Overview

Mark's Computer Build is a JavaFX application designed to manage computer builds. It interacts with a PostgreSQL database to perform CRUD operations (Create, Read, Update, Delete) on computer build records. The application allows users to add, edit, and remove computer builds, and view them in a table format.

## Features

- **Add New Computer Build**: Users can add new computer builds by filling out a form with details such as title, case type, motherboard, CPU, etc.
- **Edit Existing Computer Build**: Users can edit details of an existing computer build.
- **Remove Computer Build**: Users can delete computer builds from the database.
- **View Computer Builds**: A table view displays all the computer builds stored in the database.

## Example

Watch this [video](https://youtu.be/7iMYKnnWWLA) to see the Computer Build Manager in action:

[![Watch the video](https://img.youtube.com/vi/7iMYKnnWWLA/maxresdefault.jpg)](https://youtu.be/7iMYKnnWWLA)

## Requirements

- Java 11 or higher
- JavaFX 11 or higher
- PostgreSQL 11 or higher
- PostgreSQL JDBC Driver

## Setup

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/computer-build-manager.git
    ```

2. **Set Up the Database**

    - Create a PostgreSQL database named `MarksComputerBuildsDB`.
    - Run the provided SQL script to create the necessary tables.

3. **Configure the Database Connection**

    - Update the `DatabaseUtil` class in `src/utils/DatabaseUtil.java` with your PostgreSQL connection details:

      ```java
      private static final String URL = "jdbc:postgresql://localhost:5432/MarksComputerBuildsDB";
      private static final String USER = "postgres";
      private static final String PASSWORD = "your_password_here";
      ```

4. **Build the Project**

    - Use your preferred IDE (e.g., IntelliJ IDEA, Eclipse) to import the project.
    - Build the project to resolve all dependencies.

5. **Run the Application**

    - Run the `MainApp` class to start the application.

## Usage

1. **Add a Computer Build**

    - Click on the "Add" button to open the add dialog.
    - Fill in the required fields and click "OK" to save.

2. **Edit a Computer Build**

    - Select a build from the table.
    - Click on the "Edit" button to open the edit dialog.
    - Modify the details and click "OK" to save the changes.

3. **Remove a Computer Build**

    - Select a build from the table.
    - Click on the "Remove" button to delete the build.

## Contributing

Contributions are welcome! If you have suggestions or improvements, please create a pull request or open an issue.

## Acknowledgments

- JavaFX for the graphical user interface.
- PostgreSQL for the database management system.

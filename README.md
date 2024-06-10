# AirBnB Clone Project

## Description

Welcome to the AirBnB clone project! This project is the first step towards building a comprehensive web application that mimics the functionality of AirBnB. The main focus of this initial phase is to create a command interpreter to manage various AirBnB objects such as Users, Places, Cities, and more. This command interpreter will handle the creation, storage, and manipulation of these objects, setting a solid foundation for the subsequent development of the web application, including aspects like HTML/CSS templating, database storage, API creation, and front-end integration.

## Command Interpreter

The command interpreter acts as a simple, interactive shell that allows you to manage the AirBnB objects. It supports various commands to create, retrieve, update, and destroy instances of the objects.

### How to Start It

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/AirBnB_clone.git
   cd AirBnB_clone
   ```

2. **Make the command interpreter executable:**
   ```bash
   chmod +x console.py
   ```

3. **Run the command interpreter:**
   ```bash
   ./console.py
   ```
   Alternatively, you can use:
   ```bash
   python3 console.py
   ```

### How to Use It

Once you have the command interpreter running, you can use the following commands to interact with the AirBnB objects:

- **help** or **?**
  ```shell
  (hbnb) help
  ```
  Displays a list of available commands or detailed help for a specific command.

- **create <ClassName>**
  ```shell
  (hbnb) create User
  ```
  Creates a new instance of `ClassName`, saves it (to the JSON file), and prints the id.

- **show <ClassName> <id>**
  ```shell
  (hbnb) show User 1234-1234-1234
  ```
  Prints the string representation of an instance based on the class name and id.

- **destroy <ClassName> <id>**
  ```shell
  (hbnb) destroy User 1234-1234-1234
  ```
  Deletes an instance based on the class name and id (saves the change into the JSON file).

- **all [ClassName]**
  ```shell
  (hbnb) all
  (hbnb) all User
  ```
  Prints all string representations of all instances, or all instances of a class if `ClassName` is specified.

- **update <ClassName> <id> <attribute name> "<attribute value>"**
  ```shell
  (hbnb) update User 1234-1234-1234 email "newemail@example.com"
  ```
  Updates an instance based on the class name and id by adding or updating an attribute (saves the change into the JSON file).

### Examples

- **Creating a new User:**
  ```shell
  (hbnb) create User
  e4eaaaf2-d142-11e1-b3e4-080027620cdd
  ```

- **Showing a User instance:**
  ```shell
  (hbnb) show User e4eaaaf2-d142-11e1-b3e4-080027620cdd
  [User] (e4eaaaf2-d142-11e1-b3e4-080027620cdd) {'id': 'e4eaaaf2-d142-11e1-b3e4-080027620cdd', 'created_at': datetime.datetime(2023, 6, 10, 10, 0, 0, 0), 'updated_at': datetime.datetime(2023, 6, 10, 10, 0, 0, 0)}
  ```

- **Updating a User's email:**
  ```shell
  (hbnb) update User e4eaaaf2-d142-11e1-b3e4-080027620cdd email "newemail@example.com"
  ```

- **Showing all instances of User:**
  ```shell
  (hbnb) all User
  ```

- **Destroying a User instance:**
  ```shell
  (hbnb) destroy User e4eaaaf2-d142-11e1-b3e4-080027620cdd
  ```

(This README is generated with the help of GPT)

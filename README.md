# Java Notes App

## Objective
A simple command-line Notes Manager built using Java. This application allows users to:
- Add text-based notes
- View all saved notes

Notes are saved persistently in a file using Java File I/O.

## Tools Used
- Java (JDK 8 or higher)
- Eclipse IDE (or any Java IDE)
- Terminal / Command Prompt

## Features
- Add new notes
- View saved notes
- Persistent storage using `notes.txt`

## How It Works

### 1. Adding Notes
- Prompts the user to enter a note.
- The note is appended to a file named `notes.txt` using `FileWriter` in append mode.
- Each note is stored on a new line.

### 2. Viewing Notes
- Reads all notes from `notes.txt` using `BufferedReader`.
- Displays each note line-by-line.
- Handles the case when the file does not exist or is empty.

## Project Structure
```
Java-Notes-App/
├── src/
│   └── NotesApp.java  ←  Main class
├── notes.txt  ←  Auto-created at runtime when notes are added
```

## How to Run This Project

### Using Eclipse
1. Open Eclipse and create a new Java project (e.g., `NotesAppProject`).
2. Create a new class named `NotesApp`.
3. Copy and paste the code from `NotesApp.java` into the class.
4. Run the program and interact via the console.

## Sample Output

```
=== Simple Notes App ===

1. Add Note
2. View Notes
3. Exit
Choose an option: 1
Enter your note: Java FileWriter is useful to persist data.
Note saved successfully.

Choose an option: 2
=== Your Notes ===
-> Java FileWriter is useful to persist data.
```

## File Format
- Notes are stored in `notes.txt`, located in the same directory as the `.java` file.
- Each line in the file represents one note.

## Learning Outcome
- Understanding Java file handling using `FileWriter`, `FileReader`, and `BufferedReader`
- Building a menu-driven CLI application
- Implementing basic exception handling and user input handling

## Author
Chinta Lakshmi Kanth

## License
This project is created for educational purposes only.

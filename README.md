
# Notepad Application - Java Documentation

## Introduction
This documentation describes the functionality of the `App` class, which serves as the main entry point for interacting with the `Notepad` class. The program provides a command-line interface for managing text within a notepad-like environment, supporting various text operations.

## Features
The application supports the following operations:
1. **Display the text** - View all text in the notepad.
2. **Display the text from given lines** - Display text between specific line numbers.
3. **Insert the text** - Add a single line of text at a specific position.
4. **Insert Multiple lines of text** - Add multiple lines of text starting at a specific position.
5. **Delete the text** - Remove a single line of text.
6. **Delete from given lines** - Remove text between specific line numbers.
7. **Copy the text** - Copy text between specific line numbers.
8. **Paste the text** - Paste the copied text at a specific position.
9. **Undo your action** - Undo the last performed action.
10. **Redo your action** - Redo the last undone action.
11. **Exit** - Exit the application.

## Class: `App`
The `App` class contains the `main` method and interacts with the `Notepad` class.

### Dependencies
- `notepad.Notepad`: The `Notepad` class provides the underlying functionalities for text manipulation.
- `java.util.Scanner`: Used for input handling.

### Methods and Operations
#### 1. `main(String[] args)`
The main method initializes the application and provides a menu-driven interface for user interaction.

**Menu Options:**
- **Case 1:** Calls `notepad.display()` to display all text.
- **Case 2:** Accepts `startLine` and `endLine` inputs and calls `notepad.display(startLine, endLine)`.
- **Case 3:** Accepts `text` and `lineNumber`, then calls `notepad.insertLine(lineNumber, text)`.
- **Case 4:** Accepts multiple lines of text and calls `notepad.insertLine(lineNumber, textArr)`.
- **Case 5:** Deletes a specific line by calling `notepad.delete(lineNumber)`.
- **Case 6:** Deletes lines within a range by calling `notepad.delete(startLine, endLine)`.
- **Case 7:** Copies lines within a range using `notepad.copy(startLine, endLine)`.
- **Case 8:** Pastes copied text at a specific position using `notepad.paste(lineNumber)`.
- **Case 9:** Performs an undo operation by calling `notepad.undo()`.
- **Case 10:** Performs a redo operation by calling `notepad.redo()`.
- **Case 11:** Exits the application.

### Input Handling
The program uses `Scanner` for reading user input. Validations are not implemented for erroneous inputs, so care should be taken to input correct data types.

## Sample Execution
Below is an example of how the application menu looks during execution:
```
Choose your option
1. Display the text
2. Display the text from given lines
3. Insert the text
4. Insert Multiple lines of text
5. Delete the text
6. Delete from given lines
7. Copy the text
8. Paste the text
9. Undo your action
10. Redo your action
11. Exit
Enter the choice:
```

## Notes
- Ensure the `Notepad` class is correctly implemented and located in the `notepad` package.
- The initial capacity of the `Notepad` is set to 5 in the `App` class.

## Licensing
This program and its documentation are provided "as-is" without warranty of any kind.

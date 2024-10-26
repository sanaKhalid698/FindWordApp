# Find Tool

## Overview
The **Find Tool** is a Python application designed to help users search for specific text within files or directories. It uses two search methods: **Brute Force Search** and **Knuth-Morris-Pratt (KMP) Search**. This application provides a graphical user interface (GUI) using Tkinter, making it easy for users to input search terms and choose files or directories to search.

## Features
- Search for specific text in files or directories.
- Supports searching in different file formats such as `.txt`, `.log`, `.csv`, and `.md`.
- Offers options for:
  - Matching whole words only.
  - Case sensitivity (whether 'a' and 'A' are treated as the same).
- Displays search results along with the row and column where the text was found.
- Shows execution time for both search methods.

## Requirements
To run the Find Tool, you need:
- Python installed on your computer (version 3.6 or higher).
- Tkinter library (usually comes pre-installed with Python).

## How to Use
1. **Download the Code**: 
   - Clone or download the repository to your local machine.

2. **Run the Application**:
   - Open your command line (Terminal, Command Prompt, etc.).
   - Navigate to the directory where the code is saved.
   - Run the command: 
     ```bash
     python find_tool.py
     ```

3. **Using the Tool**:
   - **Find what**: Enter the text you want to search for in the provided box.
   - **Path**: Enter the file or directory path where you want to search or click the "Browse" button to select a file or directory.
   - **Match word only**: Check this box if you want to search for the whole word only (e.g., searching "cat" won't match "catalog").
   - **Case sensitive**: Check this box if you want the search to distinguish between uppercase and lowercase letters.
   - Click the **Search** button to begin the search.
   - After the search is complete, you can click **Find Next** to see the next occurrence of the search term.

4. **View Results**:
   - The application will display results in two sections: 
     - **Brute Force Search Results**: Shows where the text was found using the brute force method.
     - **KMP Search Results**: Shows results from the KMP search method.
   - Each result will show the file name, row number, and column number where the search term was found.
   - The execution time for each search method will be displayed below the results.

## Code Structure
- **Main Application Window**: The GUI is built using Tkinter, with labeled input fields and buttons for user interaction.
- **Search Functions**: The application contains two main functions for searching:
  - `brute_force_search`: Implements the brute force search method.
  - `kmp_search`: Implements the KMP search method.
- **Utilities**: Functions to validate user inputs, handle file selection, and update the display with search results.

## Example Use Case
Suppose you have a directory with several `.txt` files, and you want to find all occurrences of the word "example". You would:
1. Enter "example" in the **Find what** field.
2. Select the directory containing your text files.
3. Choose whether to match whole words and/or be case sensitive.
4. Click the **Search** button to see where "example" appears in the files.

## Troubleshooting
- If you encounter issues, ensure that the file paths you input are correct.
- Make sure the files you are searching through are in one of the supported formats.
- If you see an error message during the search, check the console for detailed error information.

## License
This project is open-source. You are free to use, modify, and distribute it as you wish.

## Contact
For any questions or feedback, feel free to reach out via email at [sanakhalid7440@gmail.com].

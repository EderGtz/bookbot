# Bookbot - Static Text Analyzer CLI

This project is a command-line interface (CLI) tool designed to perform static analysis on text files. Its primary function is to parse large bodies of text (such as books) and generate statistical reports on word count and character frequency.

The objective of this project was to practice file I/O operations, string manipulation, and data structuring (dictionaries/lists) in Python. It serves as a foundational exercise in building data processing scripts.

## Core Implementation

- **File Ingestion:** Reads local text files securely using context managers (`with open(...)`) to ensure proper resource handling.
- **Data Processing:**
    - **Word Count:** Tokenizes the text string to calculate the total number of words.
    - **Character Frequency:** Iterates through the text to build a frequency map (dictionary) of specific allowed characters, normalizing case for accuracy.
- **Sorting Algorithm:** Implements a custom sorting key to organize character data by frequency (descending order) before presentation.
- **Report Generation:** Formats the analyzed data into a clean, human-readable report in the terminal.

## Technical Highlights

- **Modular Architecture:** Separation of logic into `stats.py` (processing) and `main.py` (entry point/orchestration).
- **Command Line Arguments:** Utilizes `sys.argv` to accept dynamic file paths at runtime, making the tool reusable for any text file.
- **Error Handling:** Implements `try-except` blocks to gracefully handle invalid file paths or missing arguments.

# DailyPlaytestFolderCreator

# Automatic Folder Structure Generator

This Python script automatically creates a folder hierarchy based on the current date. It organizes data into month, session, and match categories, making it easier to maintain files in an organized structure. Once the folders are created, the script opens the relevant folder in your file explorer.

## How it Works

The script generates folders inside a predefined base directory. The folder hierarchy follows three levels:

1. **Month Folder:** This folder is named after the current month as a word (for example, `October` or `January`).
2. **Date Folder:** This folder is named using the current date formatted as `Day - Month(Number) - Year`. For instance, if the current date is October 3, 2023, the folder will be named `03 - 10 - 2023`. 
3. **Session and Match Folders:** Inside each date folder:
   - Three session folders are created: `Session 1 -`, `Session 2 -`, and `Session 3 -`.
   - Each session folder contains three match folders: `Match 1 -`, `Match 2 -`, and `Match 3 -`.

Once the script completes, it opens the date folder in your file manager.

## Example Folder Structure

For example, if you run the script on October 3, 2023, and the base directory is set to `C:\Users\User\Desktop\ProjectFolder\History`, the following structure will be created:



## Requirements

1. You need Python installed on your computer. You can download it from [python.org](https://www.python.org/).
2. Familiarity with running Python scripts in a terminal or command prompt.

## Setup and Usage

### Configure the Base Directory

By default, the script creates the folders inside the following directory:

base_directory = r"C:\Users\User\Desktop\ProjectFolder\History"

If you want the folders to be created somewhere else, replace the path in the script with your desired location. For example:
```python
base_directory = r"C:\Users\YourUsername\Desktop\WorkHistory"
``` 
Run the Script
1. Save the Python script (create_folder_structure.py) on your computer.
2. Open a terminal or command prompt.
3. Navigate to the folder where the script is saved.
4. Run the script with the following command:

# Translator Script Setup and Usage Guide

This guide will walk you through setting up a virtual environment and installing the necessary modules to run the Translator Script.

## Prerequisites

1. **Python Installation:**
   - Ensure Python 3.6 or higher is installed on your system. If not, download and install it from [python.org](https://www.python.org/downloads/).

2. **Text Editor or IDE:**
   - Use a text editor or integrated development environment (IDE) like VS Code, PyCharm, or Sublime Text.

## Setting Up the Virtual Environment

1. **Clone the Repository:**
   - Clone the repository to your local machine using Git or download it as a ZIP file and extract it.
     ```
     git clone <repository-url>
     ```

2. **Navigate to the Project Directory:**
   - Open a terminal or command prompt and change directory to where your `translate_script.py` is located.
     ```
     cd path/to/translate_script_directory
     ```

3. **Create a Virtual Environment:**
   - Create a virtual environment named `venv`. This isolates dependencies for this project.
     ```
     python -m venv venv
     ```

4. **Activate the Virtual Environment:**
   - Activate the virtual environment. On Windows:
     ```
     .\venv\Scripts\Activate.ps1
     ```
     On macOS and Linux:
     ```
     source venv/bin/activate
     ```

## Installing Dependencies

1. **Install Required Packages:**
   - Install the necessary Python packages listed in `requirements.txt`.
     ```
     pip install -r requirements.txt
     ```

## Running the Translator Script

1. **Prepare Input Files:**
   - Place the documents you want to translate into a folder. Update the `input_folder` variable in `translate_script.py` with the path to this folder.
     ```python
     input_folder = r"C:\path\to\your\input\folder"
     ```

2. **Run the Script:**
   - Execute the script to translate each document in the input folder and save the translated documents.
     ```
     python translate_script.py
     ```

## Points to Ponder

- **Google Translator API Quotas:**
  - Google Translator API has usage quotas and may incur charges based on usage. Ensure you have sufficient quota or billing enabled if translating large amounts of text.
  
- **Input Document Format:**
  - Ensure the input documents are in a format compatible with the `python-docx` library (e.g., `.docx` files). Adjust the script if handling different file formats.
  
- **Handling Errors:**
  - Monitor terminal or command prompt output for any errors or warnings during script execution. Refer to logs or error messages to diagnose issues.

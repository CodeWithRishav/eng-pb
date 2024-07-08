<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Translator Script Setup and Usage Guide</title>
</head>
<body>
    <h1>Translator Script Setup and Usage Guide</h1>

    <p>This guide will walk you through setting up a virtual environment and installing the necessary modules to run the Translator Script.</p>

    <h2>Prerequisites</h2>

    <ol>
        <li><strong>Python Installation:</strong>
            <ul>
                <li>Ensure Python 3.6 or higher is installed on your system. If not, download and install it from <a href="https://www.python.org/downloads/">python.org</a>.</li>
            </ul>
        </li>
        <li><strong>Text Editor or IDE:</strong>
            <ul>
                <li>Use a text editor or integrated development environment (IDE) like VS Code, PyCharm, or Sublime Text.</li>
            </ul>
        </li>
    </ol>

    <h2>Setting Up the Virtual Environment</h2>

    <ol>
        <li><strong>Clone the Repository:</strong>
            <ul>
                <li>Clone the repository to your local machine using Git or download it as a ZIP file and extract it.</li>
                <li><code>git clone &lt;repository-url&gt;</code></li>
            </ul>
        </li>
        <li><strong>Navigate to the Project Directory:</strong>
            <ul>
                <li>Open a terminal or command prompt and change directory to where your <code>translate_script.py</code> is located.</li>
                <li><code>cd path/to/translate_script_directory</code></li>
            </ul>
        </li>
        <li><strong>Create a Virtual Environment:</strong>
            <ul>
                <li>Create a virtual environment named <code>venv</code>. This isolates dependencies for this project.</li>
                <li><code>python -m venv venv</code></li>
            </ul>
        </li>
        <li><strong>Activate the Virtual Environment:</strong>
            <ul>
                <li>Activate the virtual environment. On Windows:</li>
                <li><code>.\venv\Scripts\Activate.ps1</code></li>
                <li>On macOS and Linux:</li>
                <li><code>source venv/bin/activate</code></li>
            </ul>
        </li>
    </ol>

    <h2>Installing Dependencies</h2>

    <ol>
        <li><strong>Install Required Packages:</strong>
            <ul>
                <li>Install the necessary Python packages listed in <code>requirements.txt</code>.</li>
                <li><code>pip install -r requirements.txt</code></li>
            </ul>
        </li>
    </ol>

    <h2>Running the Translator Script</h2>

    <ol>
        <li><strong>Prepare Input Files:</strong>
            <ul>
                <li>Place the documents you want to translate into a folder. Update the <code>input_folder</code> variable in <code>translate_script.py</code> with the path to this folder.</li>
                <li><code>input_folder = r"C:\path\to\your\input\folder"</code></li>
            </ul>
        </li>
        <li><strong>Run the Script:</strong>
            <ul>
                <li>Execute the script to translate each document in the input folder and save the translated documents.</li>
                <li><code>python translate_script.py</code></li>
            </ul>
        </li>
    </ol>

    <h2>Points to Ponder</h2>

    <ul>
        <li><strong>Google Translator API Quotas:</strong>
            <ul>
                <li>Google Translator API has usage quotas and may incur charges based on usage. Ensure you have sufficient quota or billing enabled if translating large amounts of text.</li>
            </ul>
        </li>
        <li><strong>Input Document Format:</strong>
            <ul>
                <li>Ensure the input documents are in a format compatible with the <code>python-docx</code> library (e.g., <code>.docx</code> files). Adjust the script if handling different file formats.</li>
            </ul>
        </li>
        <li><strong>Handling Errors:</strong>
            <ul>
                <li>Monitor terminal or command prompt output for any errors or warnings during script execution. Refer to logs or error messages to diagnose issues.</li>
            </ul>
        </li>
    </ul>

</body>
</html>

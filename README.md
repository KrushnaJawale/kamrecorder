Kam Recorder
A local recording studio for creators who want camera recording, screen capture, playback, and an AI-assisted teleprompter in one practical tool.

About the project
Kam Recorder is shared so you can learn from it, use it locally, and change the code to fit your own workflow.

Camera recording
Screen recording
Hybrid camera and screen recording
Folder-based media storage
In-app video playback
Teleprompter controls and scrolling
AI script generation
Groq API key management
Requirements
Windows
Python 3
Python added to the system PATH
A Groq API key for AI script generation
The teleprompter uses the openai/gpt-oss-20b open model through the Groq API. Recording and the teleprompter can still be used without configuring an AI key.

Installation
1. Install Python
Download Python from python.org. During installation, enable Add Python to PATH so the terminal can find Python and pip.

2. Open the project folder
Open Command Prompt or PowerShell and move into the project directory:

cd "C:\path\to\Studio-Recorder-Pro"
Replace the example path with the folder where you saved this project.

3. Install dependencies
Run this command in the project folder:

pip install -r requirements.txt
4. Start the application
After installation finishes, run the included Windows startup script:

run.bat
The script starts the Flask server and opens the application in your browser automatically. The local address may be different on your computer, so use the address opened by the script. Keep the server window open while using the application.

Using the AI teleprompter
Open Connect Groq in the app.
Add your Groq API key.
Select the key in the teleprompter panel.
Enter a prompt and generate your script.
Start the teleprompter when your script is ready.
API keys are stored in the local SQLite database. Do not share your database.db file or publish API keys in screenshots, commits, or public repositories.

Customize the project
You are welcome to edit the source code for your own needs. You can change the interface, recording behavior, API integration, startup process, and teleprompter model. You may replace the current model or provider in app.py, but review the provider's terms and keep credentials private.

templates/index.html   Main recording studio interface
templates/creator.html  Creator profile page
templates/groq.html     Groq API key management
app.py                  Flask application and API routes
requirements.txt        Python dependencies
run.bat                 Windows startup script
recordings/             Saved camera and screen recordings
Creator
I am Krushna Jawale. I like building this kind of software, especially tools that combine recording, productivity, and practical AI workflows.

See more of my work at krushnajawale.vercel.app.

Usage and redistribution
This project is provided for learning, personal use, and modification. You may edit the source code and create your own private versions.

Paid redistribution, resale, or presenting this tool as a paid product is strictly prohibited. You may not sell the original project, a lightly modified version, packaged access to it, or a service whose primary purpose is reselling this tool. Suspected commercial misuse may be reported and may result in legal action where applicable.
Please respect the terms of Python, Flask, Groq, the openai/gpt-oss-20b model, and any other third-party services or components used with your modified version.

Disclaimer
This is a local creator tool provided as-is. You are responsible for your API keys, recordings, uploaded content, configuration, and compliance with the terms of any third-party service you connect to it.

Kam Recorder documentation · Krushna Jawale

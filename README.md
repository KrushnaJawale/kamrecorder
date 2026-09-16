<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Kam Recorder | Documentation</title>

</head>
<body>
<main class="docs">
<header class="hero">
<h1>Kam Recorder</h1>
<p class="tagline">A local recording studio for creators who want camera recording, screen capture, playback, and an AI-assisted teleprompter in one practical tool.</p>
</header>

<section>
<h2>About the project</h2>
<p>Kam Recorder is shared so you can learn from it, use it locally, and change the code to fit your own workflow.</p>
<div class="grid"><ul><li>Camera recording</li><li>Screen recording</li><li>Hybrid camera and screen recording</li><li>Folder-based media storage</li></ul><ul><li>In-app video playback</li><li>Teleprompter controls and scrolling</li><li>AI script generation</li><li>Groq API key management</li></ul></div>
</section>

<section>
<h2>Requirements</h2>
<ul><li>Windows</li><li>Python 3</li><li>Python added to the system <strong>PATH</strong></li><li>A Groq API key for AI script generation</li></ul>
<p>The teleprompter uses the <strong>openai/gpt-oss-20b</strong> open model through the Groq API. Recording and the teleprompter can still be used without configuring an AI key.</p>
</section>

<section>
<h2>Installation</h2>
<h3>1. Install Python</h3>
<p>Download Python from <a href="https://www.python.org/downloads/" target="_blank" rel="noreferrer">python.org</a>. During installation, enable <strong>Add Python to PATH</strong> so the terminal can find Python and pip.</p>
<h3>2. Open the project folder</h3>
<p>Open Command Prompt or PowerShell and move into the project directory:</p>
<div class="code">cd "C:\path\to\Studio-Recorder-Pro"</div>
<p>Replace the example path with the folder where you saved this project.</p>
<h3>3. Install dependencies</h3>
<p>Run this command in the project folder:</p>
<div class="code">pip install -r requirements.txt</div>
<h3>4. Start the application</h3>
<p>After installation finishes, run the included Windows startup script:</p>
<div class="code">run.bat</div>
<p>The script starts the Flask server and opens the application in your browser automatically. The local address may be different on your computer, so use the address opened by the script. Keep the server window open while using the application.</p>
</section>

<section>
<h2>Using the AI teleprompter</h2>
<ol><li>Open <strong>Connect Groq</strong> in the app.</li><li>Add your Groq API key.</li><li>Select the key in the teleprompter panel.</li><li>Enter a prompt and generate your script.</li><li>Start the teleprompter when your script is ready.</li></ol>
<p class="notice">API keys are stored in the local SQLite database. Do not share your <strong>database.db</strong> file or publish API keys in screenshots, commits, or public repositories.</p>
</section>

<section>
<h2>Customize the project</h2>
<p>You are welcome to edit the source code for your own needs. You can change the interface, recording behavior, API integration, startup process, and teleprompter model. You may replace the current model or provider in <strong>app.py</strong>, but review the provider's terms and keep credentials private.</p>
<div class="code">templates/index.html   Main recording studio interface
templates/creator.html  Creator profile page
templates/groq.html     Groq API key management
app.py                  Flask application and API routes
requirements.txt        Python dependencies
run.bat                 Windows startup script
recordings/             Saved camera and screen recordings</div>
</section>

<section>
<h2>Creator</h2>
<p>I am <strong>Krushna Jawale</strong>. I like building this kind of software, especially tools that combine recording, productivity, and practical AI workflows.</p>
<p>See more of my work at <a href="https://krushnajawale.vercel.app" target="_blank" rel="noreferrer">krushnajawale.vercel.app</a>.</p>
</section>

<section>
<h2>Usage and redistribution</h2>
<p>This project is provided for learning, personal use, and modification. You may edit the source code and create your own private versions.</p>
<div class="warning"><strong>Paid redistribution, resale, or presenting this tool as a paid product is strictly prohibited.</strong> You may not sell the original project, a lightly modified version, packaged access to it, or a service whose primary purpose is reselling this tool. Suspected commercial misuse may be reported and may result in legal action where applicable.</div>
<p>Please respect the terms of Python, Flask, Groq, the <strong>openai/gpt-oss-20b</strong> model, and any other third-party services or components used with your modified version.</p>
</section>

<section>
<h2>Disclaimer</h2>
<p>This is a local creator tool provided as-is. You are responsible for your API keys, recordings, uploaded content, configuration, and compliance with the terms of any third-party service you connect to it.</p>
</section>
<footer>Kam Recorder documentation · Krushna Jawale</footer>
</main>
</body>
</html>

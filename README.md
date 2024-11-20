<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <h1>Parti ViewBot</h1>
    <h2>Overview</h2>
    <p><strong>Parti ViewBot</strong> is a tool designed to fetch and analyze livestream viewer data from 
    <a href="https://parti.com">Parti.com</a> to identify potential view botting activities. 
    This project is currently in <strong>Beta Testing (v0.1A)</strong> and serves as a proof of concept while the algorithms are still under development.</p>
    <h2>Features</h2>
    <ul>
        <li>Fetch livestream channel data using Parti.com API.</li>
        <li>Analyze viewer count to estimate the proportion of real and bot viewers.</li>
        <li>Save the analyzed data in a structured JSON file.</li>
        <li>Easy to use with minimal setup.</li>
    </ul>
    <h2>Installation</h2>
    <ol>
        <li>Clone the repository:
            <pre><code>git clone https://github.com/Riotcoke123/partiviewbot.git</code></pre>
        </li>
        <li>Navigate to the project directory:
            <pre><code>cd partiviewbot</code></pre>
        </li>
        <li>Install the required dependencies:
            <pre><code>pip install requests</code></pre>
        </li>
    </ol>
    <h2>Usage</h2>
    <ol>
        <li>Open the <code>main.py</code> file and set the <code>user_id</code> to the ID of the Parti.com user you want to analyze.</li>
        <li>Run the script:
            <pre><code>python main.py</code></pre>
        </li>
        <li>The script will fetch data from the Parti.com API, analyze the viewer counts, and save the results to a JSON file. By default, the output file is named <code>bot.json</code> and located on your desktop.</li>
    </ol>
    <h2>JSON Output</h2>
    <p>The JSON file contains the following fields:</p>
    <ul>
        <li><code>id</code>: The user ID of the channel.</li>
        <li><code>viewer_count</code>: Total number of viewers in the stream.</li>
        <li><code>real_viewer_count</code>: Estimated number of real viewers.</li>
        <li><code>bot_viewer_count</code>: Estimated number of bot viewers.</li>
    </ul>
    <h3>Example Output</h3>
    <pre><code>{
    "id": "352497",
    "viewer_count": 500,
    "real_viewer_count": 100,
    "bot_viewer_count": 400
}</code></pre>
    <h2>Roadmap</h2>
    <ul>
        <li>Improve the algorithm for detecting real vs. bot viewers.</li>
        <li>Add support for analyzing historical data.</li>
        <li>Create a web interface for visualization.</li>
        <li>Expand compatibility to include additional streaming platforms.</li>
    </ul>
    <h2>Contribution</h2>
    <p>Contributions are welcome! Please fork the repository, make your changes, and submit a pull request. 
    Ensure your code adheres to the existing style and passes any tests.</p>
    <h2>License</h2>
    <p>This project is licensed under the MIT License. See the <a href="https://github.com/Riotcoke123/partiviewbot/blob/main/LICENSE">LICENSE</a> file for details.</p>
    <h2>Disclaimer</h2>
    <p>This tool is for educational and research purposes only. Please use it responsibly and in compliance with 
    <a href="https://parti.com">Parti.com's</a> terms of service.</p>
</body>
</html>

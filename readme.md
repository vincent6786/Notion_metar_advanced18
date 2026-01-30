✈️ METAR Go
A lightweight, pilot-focused Electronic Flight Bag (EFB) web application.

METAR PLUS Pro is a single-file web tool designed for student pilots and aviation enthusiasts. It provides instant access to real-time aviation weather, runway analysis, and flight planning tools in a "Cockpit Night Mode" friendly interface.

🌟 Key Features
Real-Time Weather: Decodes and displays raw METAR & TAF data from AVWX.

Visual Flight Rules (VFR) Status: Instant color-coded badges (VFR, MVFR, IFR, LIFR).

Runway Analysis:

Dynamic Wind Rose visualizing headwind/crosswind components.

Automatic "Best Runway" suggestion based on current winds.

Smart World Clock:

Search by City Name (e.g., "Paris") or ICAO (e.g., "LFPG").

Automatically detects timezones using coordinates (no database required).

Displays Zulu (UTC) offset (e.g., "UTC +8").

Failover Network System: Built-in "Smart Fetch" automatically rotates through multiple API keys if one limit is reached (Error 429).

Pilot Tools:

E6B Computer: Calculate Density Altitude & True Airspeed (TAS).

Personal Minimums: Set your own Crosswind/Ceiling limits; the app warns you if conditions are "NO-GO".

Cockpit Night Mode: One-tap toggle to switch the entire UI to a low-light Red/Black theme to preserve night vision.

🚀 Getting Started
Since this is a Single File Application, installation is incredibly simple.

Prerequisites
A modern web browser (Chrome, Safari, Edge).

(Optional) An account with AVWX to generate your own API keys.

Installation
Download the index.html file from this repository.

Open the file directly in your browser.

Deploy (Recommended): Upload the file to Vercel, Netlify, or GitHub Pages to access it from any device via a URL.

⚙️ Configuration
To ensure the app works reliably, you should add your own API keys.

Open index.html in a text editor (VS Code, Notepad, TextEdit).

Scroll down to the <script> section (approx. line 600).

Locate the API_KEYS array:

JavaScript
// SECURITY NOTE: Keys rotate automatically if one hits the limit.
const API_KEYS = [
    'YOUR_KEY_1_HERE',
    'YOUR_KEY_2_HERE',
    'YOUR_KEY_3_HERE'
];
Replace the placeholder strings with your actual AVWX tokens.

📱 Mobile Installation (PWA)
This app is Progressive Web App (PWA) ready.

On iOS (iPhone/iPad):

Open the website in Safari.

Tap the Share button (Square with arrow).

Select "Add to Home Screen".

Result: The app launches full-screen without the browser URL bar, just like a native app.

On Android:

Open in Chrome.

Tap the menu (three dots) -> "Install App".

🛠️ Technologies Used
HTML5 / CSS3 / Vanilla JavaScript: Zero dependencies, lightweight, and fast.

AVWX API: The primary source for global aviation weather data.

Open-Meteo API: Used for weather graphs and automatic timezone resolution.

Local Storage: Saves your preferences (Night Mode, History, World Clock cities) directly to your device.

⚠️ Disclaimer
FOR SIMULATION AND SITUATIONAL AWARENESS ONLY.

This software is provided "as is", without warranty of any kind. It is not a certified source of aviation weather. Pilots in Command (PIC) must always verify weather data via official sources (e.g., FSS, ForeFlight, Official Briefings) before flight operations.

Fly Safe! ✈️

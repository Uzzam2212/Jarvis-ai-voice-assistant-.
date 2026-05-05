Jarvis is a sophisticated personal AI assistant built in Python. It bridges the gap between human voice and machine execution, allowing users to control their desktop environment, manage web workflows, and automate repetitive tasks through natural language.
🏗️ Architecture & Logic
Jarvis is built with modularity at its core. Instead of a single monolithic script, the system uses a provider-based architecture:
The Listener (STT): Utilizes the SpeechRecognition library to interface with the Google Web Speech API, converting audio input into actionable strings.
The Brain (NLP): A central command-parsing engine that utilizes string matching and keyword extraction to determine user intent.
The Voice (TTS): Powered by pyttsx3, providing a low-latency, offline-capable text-to-speech synthesis that works cross-platform.
Skill Modules: A decoupled directory of scripts where each "skill" (Weather, Email, System Control) lives independently.
🚀 Core Features
1. System Automation
Application Control: Launch or terminate software like VS Code, Chrome, or Spotify.
Hardware Management: Voice commands for system volume, battery status, and screen brightness.
File Navigation: Open specific project folders or documents instantly.
2. Web & Productivity
Smart Search: "Jarvis, search Google for..." or "Who is..." pulls data from Google and Wikipedia.
Media Playback: Full voice control for YouTube and music streaming.
Real-time Updates: Fetch current weather, top news headlines, or time/date across time zones.
3. Developer Tools
GitHub Integration: Quick links to open repositories or check status.
Automation: Set reminders or timers to manage "Deep Work" sessions.
🛠️ Installation & Setup
Prerequisites
Python 3.10 or higher.
Active Internet connection (for Google STT).
PyAudio (requires portaudio for non-Windows systems).

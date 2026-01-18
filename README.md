
🤖 DroidSync-Vision-Agent
DroidSync is an autonomous AI agent built on the Droidrun Framework. It uses computer vision to "see" and "think" like a human employee, navigating between multiple apps to automate complex scheduling workflows without needing any backend APIs.

🚀 The Challenge: Cross-App Data Synthesis
The agent was tasked with a high-complexity workflow:

Identify & Extract: Autonomously open Gmail, locate the latest meeting-related email, and parse unstructured date/time data.

Context Retention: "Remember" the extracted details while transitioning between apps.

Action Execution: Open the System Calendar, create a "Work Sync" event at the exact extracted time, and save it.

Active Alerting: The system ensures the Calendar event is saved with a Reminder/Notification, so the user never misses a sync.

🛠️ How it Works (Step-by-Step)
1. Vision-Based Perception
Unlike traditional bots that use element IDs, DroidSync uses Google Gemini Vision via Mobilerun Cloud to recognize app icons and text on the screen. It can handle UI changes or unexpected pop-ups autonomously.

2. Intelligent Reasoning
The agent reads the email content and uses natural language processing to understand phrases like "See you tomorrow at 4 PM" and converts them into a valid system timestamp.

3. Automated Scheduling & Notification
Once the event is saved in the Calendar, the agent verifies the entry. Because it interacts with the native Android Calendar, you will automatically receive a system notification before the meeting starts, ensuring a 100% reliable productivity loop.

📊 Technical Stack
Language: Python 3.13

Framework: Droidrun

Infrastructure: Mobilerun Cloud (High-scale Vision Processing)

Connection: ADB (Android Debug Bridge)

🔧 Installation & Setup
Connect Device: Ensure USB Debugging is ON and adb devices shows your serial number.

Environment:

Bash

$env:GOOGLE_API_KEY="your_api_key_here"
Execute:

Bash

python DroidAgent.py
💡 Why this is a B2B Power Tool
In a corporate environment, manual scheduling takes up 15% of an employee's time. DroidSync eliminates this by acting as a "Digital Twin" that handles the logistics, while the system notifications keep the employee on track.

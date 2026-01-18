# 🤖 **DroidSync-Vision-Agent**

## 🌟 **Project Overview**
Our agent is a **Vision-based AI** that performs tasks autonomously. Without relying on traditional APIs, it "sees" the screen like a human and switches between apps to complete workflows.



## 💡 **Why is this Important? (The "Difficult" Part)**
Most automation tools (like Zapier or Selenium) require backend access or fixed element IDs. **DroidSync-Vision-Agent** is unique for the following reasons:
* **Zero API Dependency**: Works on any app without needing official API access.
* **Vision Over Code**: Resilient to UI changes; identifies elements visually.
* **Complex Data Reasoning**: Handles unstructured date/time extraction from emails.
* **B2B Impact**: Automates manual scheduling, saving significant employee time.

## 🛠️ **Key Steps in Automation**
1. **Gmail Data Extraction**: The agent identifies the specific message containing 'Meeting'.
2. **Contextual Reasoning**: It extracts the **Date and Time** and stores it in memory.
3. **Calendar Integration**: It opens the **System Calendar** and creates the event.
4. **Smart Notification**: The native **Calendar app triggers a notification** once saved.

## 🔧 **Installation & Setup (Crucial Steps)**

Follow these steps to get the agent running on your local machine:

### **1. Prerequisites**
* **Python 3.13+**: Ensure you have the latest Python version installed.
* **ADB Tools**: Install Android Debug Bridge and add it to your System Path.
* **Mobile Device**: Enable **USB Debugging** on your Android phone.

### **2. Clone and Install**
```bash
# Clone the repository
git clone [https://github.com/yourusername/DroidSync-Vision-Agent.git](https://github.com/yourusername/DroidSync-Vision-Agent.git)
cd DroidSync-Vision-Agent'''

2. Device Connection (ADB)
The agent communicates with your device via the Android Debug Bridge (ADB):

Enable Developer Options and USB Debugging on your Android phone.

Connect the phone to your PC.

Verify the connection by running:

Bash

adb devices
🚀 Execution Flow & Verification
Execution Flow
To launch the autonomous agent, run the following command in your terminal:

Bash

python main.py
Process Cycle
Screenshot: The agent captures the current screen state.

Vision Analysis: Screenshots are processed via Mobilerun Cloud to understand the UI.

Action Planning: The AI plans the next tap or swipe based on your prompt.

Device Command: Commands are sent to the phone via ADB.

Verification (How to check success)
Terminal Logs: Monitor the logs for "Action: Clicking Gmail" or "Action: Typing in Calendar".

Visual Confirmation: Watch your phone screen; it will navigate Gmail and Calendar without manual input.

Final Output: Check your Calendar app for the 'Work Sync' event. You will receive a system notification.

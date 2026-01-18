# 🤖 **DroidSync-Vision-Agent**

## 🌟 **Project Overview**
Our agent is a **Vision-based AI** that performs tasks autonomously. Without relying on traditional APIs, it "sees" the screen like a human and switches between apps to complete workflows.
## 📺 **Project Demo Video**
Click the image below to watch the full 3-minute demo of the Vision Agent in action:

[![Watch the video]

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
## 🔧 **Detailed Configuration & Execution**

### **2. Environment Setup**
Create a `.env` file in your project folder and add your key.
```env
GOOGLE_API_KEY=your_actual_api_key_here
```

### **3. Device Connection (ADB)**
The agent communicates with your device via the Android Debug Bridge (ADB):
* **Step A:** Enable Developer Options and USB Debugging on your phone.
* **Step B:** Connect your phone to your PC via USB.
* **Step C:** Verify the connection by running:
```bash
adb devices
```

### 🚀 **4.Execution Flow & Verification**
Execution Flow
Run the main script to start the automation:
```bash

python main.py
```
### **5.Verification (How to check success)**
**Terminal Logs**: Monitor the logs for **"Action: Clicking Gmail"**

**Visual Confirmation**: Watch your phone screen navigate autonomously.

**Final Output**: You will see a **system notification from your Calendar app** 

## 🛠️ **Tech Stack**

* **Language**: Python 3.13+
* **AI Model**: Google Gemini (Vision Capabilities) 
* **Device Control**: ADB (Android Debug Bridge)
* **Environment Management**: Python-dotenv (for secure API keys)


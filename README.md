# -Smart-Scheduler-AI-Agent-with-n8n
🧠 Smart Scheduler AI Agent (n8n + Google Gemini + Google Calendar)

This project is an AI-powered scheduling agent built using n8n, Google Gemini (LLM), and Google Calendar. It interprets natural language chat messages like “Schedule a meeting tomorrow at 3 PM” and automatically creates calendar events, all without manual input.

🛠️ Key Features

Chat-based scheduling via natural language

Google Gemini integration for intent understanding

Contextual memory using Simple Memory

Conflict detection with Google Calendar

Fully automated event creation

📸 Workflow Overview

Here’s what the n8n workflow looks like:


Flow breakdown:

When chat message received — starts the flow when a user sends a message

AI Agent — acts as the brain, calling:

Google Gemini Chat Model to understand intent

Simple Memory for contextual understanding

Google Calendar to get existing events and schedule new ones

🧪 Example Prompt

User input:

Schedule a call with Sarah on 20 June 2025 at 3:00 PM

Output from the AI Agent:

Great! I’m scheduling your meeting now. You should receive a confirmation email shortly. Is there anything else I can help with?

🧰 Tech Stack

n8n (Low-code workflow automation)

Google Gemini (Large Language Model)

Google Calendar API (event management)

Simple Memory (context store)

📦 Getting Started

Clone this repository:

git clone https://github.com/yourusername/smart-scheduler-agent.git

Import the workflow file into n8n:

Open n8n

Go to “My workflows”

Click the plus ➕ and choose Import from file

Select smart_scheduler_workflow.json

Set up your credentials:

Gemini API Key

Google Calendar API with OAuth2

Create a .env file based on .env.example

Start your n8n instance and test it by sending a chat message.

🧩 Environment Variables

Create a .env file and define the following:

GEMINI_API_KEY=your_gemini_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_REFRESH_TOKEN=your_refresh_token

📂 Folder Structure

.
├── workflows/
│ └── smart_scheduler_workflow.json
├── assets/
│ └── workflow-screenshot.png
├── .env.example
├── README.md
└── LICENSE

🧑‍⚖️ License

MIT License. Feel free to use, modify, and share.

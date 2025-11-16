AI-Powered Local Language Health Advisor

A smart, cross-platform desktop assistant that helps users understand symptoms, medical terms, prescriptions, and health-related content — in their local languages like Hindi, Marathi, Tamil, Telugu, and English.

This tool works by analyzing text, screenshots, audio, and contextual chat, providing clear explanations, possible conditions (not diagnosis), and helpful insights.

The app supports both local/offline AI (Ollama) and online cloud AI (Google Gemini).

🚀 Quick Start Guide
Prerequisites

Node.js installed

Git installed

Choose ONE AI provider:

Google Gemini API (online, fast, accurate)

Ollama (offline, privacy-focused, recommended)

📥 Installation
1. Clone the repository
git clone [repository-url]
cd free-cluely

2. Install dependencies

If you face Sharp/Python build errors:

SHARP_IGNORE_GLOBAL_LIBVIPS=1 npm install --ignore-scripts
npm rebuild sharp


Or normal installation:

npm install

🔧 Environment Setup

Create a .env file in the project root.

Option A — Use Gemini
GEMINI_API_KEY=your_api_key_here

Option B — Use Ollama (Offline)
USE_OLLAMA=true
OLLAMA_MODEL=llama3.2
OLLAMA_URL=http://localhost:11434


Make sure Ollama is installed and running if you choose this option.

▶️ Running the Application
Development Mode (recommended first run)
npm start


This auto-starts:

Vite server (port 5180)

Electron app

Production Build
npm run dist


Output will be in the release/ folder.

🤖 AI Provider Options
Ollama (Offline & Private — Recommended)

100% local processing

Works without internet

Supports models like:

llama3.2

mistral

codellama

No API cost

Setup:

ollama pull llama3.2
ollama serve

Google Gemini (Cloud)

Most accurate

Best reasoning

Fast

Costs depend on usage

Get API key from Google AI Studio.

⚠️ Important Notes
Quitting the App

Windows/Linux: Ctrl + Q

macOS: Cmd + Q

(X button known issue)

Port Issues

If 5180 is busy:

lsof -i :5180
kill [PID]

Common Build Fix
rm -rf node_modules package-lock.json
npm install

✨ Key Features (Health-Focused)
🩺 1. Symptom & Health Query Understanding

Ask questions in local languages — Hindi, Marathi, Telugu, Tamil, English:

“मुझे चक्कर क्यों आ रहे हैं?”

“గొంతు నొప్పి కి కారణాలు ఏవి?”

“Fever 2 days + body pain — what does it mean?”

AI provides:

Possible conditions (not diagnosis)

Home-care guidance

Explanation in simple language

📸 2. Smart Screenshot Analysis

Analyze screenshots of:

Prescriptions

Medical reports

Symptoms described in images

Test results

Doctor notes

Shortcut: Cmd/Ctrl + H

🎧 3. Audio Health Explanation

Upload audio/speech explaining your symptoms:

Converts to text

Analyzes content

Gives clear interpretation

💬 4. Contextual Chat

Continue asking questions without losing previous context.

🔒 5. Privacy-First Design

Offline mode supported using Ollama

No data stored

Screenshots auto-deleted

No tracking

🌍 Cross-Platform Support

Windows 10/11

macOS

Linux (Ubuntu + others)

🧪 Use Cases
For Students

✓ Explaining biology/health topics
✓ Translation of complex health terms
✓ Interactive learning

For Families

✓ Understanding prescriptions
✓ Clarifying symptoms
✓ Health-related guidance in local languages

For Professionals

✓ AI assistance for documentation
✓ Quick symptom review
✓ Language support during patient communication

🔧 System Requirements

Minimum:

4GB RAM

Dual-core CPU

Recommended:

8GB+ RAM

Quad-core CPU

Optimal:

16GB RAM (for offline AI models)

🤝 Contributing

You are welcome to contribute:

Bug fixes

New AI model integration

Language improvements

Better health-related responses

UI/UX updates

📄 License

Apache-2.0 — Free for personal & commercial use.
### 🏷️ Tags
`ai-assistant` `meeting-notes` `interview-helper` `presentation-support` `ollama` `gemini-ai` `electron-app` `cross-platform` `privacy-focused` `open-source` `local-ai` `screenshot-analysis` `academic-helper` `sales-assistant` `coding-companion`

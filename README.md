# AI-quiz-apc-project

# 🎮 AI Quiz Generator 2.0 — Neon Learning Lab

A gaming-inspired desktop quiz application built with **Python and pywebview**, designed to make learning interactive, engaging, and fun. Generate AI-powered quizzes, test your knowledge, upload study materials, and track your progress through a modern neon-themed interface.

## ✨ Features

- 🎨 **Neon UI:** Modern dark dashboard with a gaming-inspired design.
- 🤖 **AI-Powered Quizzes:** Generate quizzes on custom topics using OpenAI's `gpt-4o-mini`.
- 📚 **Study Material Upload:** Upload PDF, DOCX, and TXT files to generate topic-specific questions.
- 🔒 **Source-Only Mode:** Questions generated from uploaded materials must include evidence from the extracted content.
- ⏱️ **Quiz Timer:** Challenge yourself with timed quizzes.
- 🎯 **Instant Feedback:** Review answers and learn from mistakes.
- 📊 **Results & Progress:** View quiz scores and track your performance.
- 📝 **Answer Review:** Review questions, correct answers, and your responses.
- 📜 **Quiz History:** Store past quiz attempts locally in `data/history.json`.
- 📴 **Offline Mode:** Practice using the built-in Python, Physics, and Biology question banks.
- 🛡️ **Safe Fallback:** Uploaded-material mode does not silently replace source-based questions with general-knowledge questions.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.10+ | Application logic |
| pywebview | Desktop application window |
| HTML, CSS & JavaScript | User interface |
| OpenAI API | AI-powered quiz generation |
| JSON | Local quiz history storage |
| PDF, DOCX & TXT parsers | Study material extraction |

## 📁 Project Overview

The application includes the following major components:

- **Application Backend:** Handles quiz logic, AI requests, and desktop integration.
- **Frontend Interface:** Provides the dashboard, quiz screens, results, and history views.
- **Study Material Processing:** Extracts text from supported document formats.
- **Question Bank:** Supplies offline practice questions for supported subjects.
- **Local Storage:** Saves quiz history in JSON format.

*Refer to the project files for the exact directory structure.*

## 🚀 Getting Started

### Prerequisites

- Python 3.10 or newer
- pip package manager
- An OpenAI API key for AI-powered quiz generation

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <your-project-folder>
```

### 2. Install Dependencies

Open PowerShell in the project directory and run:

```powershell
py -m pip install -r requirements.txt
```

### 3. Configure the API Key

AI-powered features require an OpenAI API key.

Set the key in your current PowerShell session:

```powershell
$env:OPENAI_API_KEY="your_api_key_here"
```

Replace the placeholder with your own API key. Never commit API keys to GitHub or include them in source code.

### 4. Run the Application

```powershell
py main.py
```

Keep the terminal open while using the application.

## 🎓 Available Modes

### AI Quiz Mode
Enter a topic and generate questions using the configured OpenAI model.

### Study Material Mode
Upload a PDF, DOCX, or TXT file and generate questions grounded in its extracted content. This mode requires an API key and validates questions against the uploaded material.

### Offline Practice Mode
Practice using the bundled question banks for:

- Python
- Physics
- Biology

Offline mode does not require an OpenAI API key.

## 📈 Quiz

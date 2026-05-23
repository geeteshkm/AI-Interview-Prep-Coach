# Zephyr - AI Interview Prep Coach

An AI-powered mock interview simulator built with Python, Streamlit, and Google Gemini API. Zephyr simulates real HR and technical interview questions, evaluates your answers, and gives personalized feedback to help you improve communication, confidence, and interview performance.

---

## 🎯 Features

- **Mock Interview Simulation**: Choose from real HR and technical interview questions
- **AI-Powered Feedback**: Google Gemini API evaluates your answer and gives detailed, personalized coaching
- **Instant Response Analysis**: Feedback is generated in real-time after you submit your answer
- **Resume Tips Module**: Built-in guidance to help users improve their resume alongside interview skills
- **Modular Architecture**: Separate modules for chatbot logic, feedback engine, and question bank for easy extension
- **Beginner Friendly UI**: Clean Streamlit interface — no login, no setup friction

---

## Screenshots

![App Screenshot](screenshots/zephyr3.png)
![App Screenshot](screenshots/zephyr4.png)

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | Streamlit |
| **AI / LLM** | Google Gemini API (gemini-1.5-flash) |
| **Backend Logic** | Python |
| **Question Bank** | JSON |
| **Environment** | python-dotenv |

---

## 📁 Project Structure

```
AI-Interview-Prep-Coach/
│
├── app.py                   # Main Streamlit app — UI and user flow
├── chatbot.py               # Gemini API integration and prompt logic
├── feedback_engine.py       # Answer evaluation and feedback formatting
├── resume_tips.py           # Resume improvement suggestions module
├── question_bank.json       # HR and technical question database
├── requirements.txt         # Python dependencies
├── .gitignore               # Excludes .env and cache files
├── screenshots/             # App screenshots for README
└── README.md                # This file
```

## 📋 Prerequisites

- **Python**: 3.9 or higher
- **Google Gemini API Key**: Free from [Google AI Studio](https://aistudio.google.com)

---

## 🚀 Setup & Run (A-Z)

### Step 1: Clone the Repository
```
git clone https://github.com/geeteshkm/AI-Interview-Prep-Coach.git
cd AI-Interview-Prep-Coach
```
### Step 2: Install Dependencies
```
pip install -r requirements.txt
```
### Step 3: Add Your Gemini API Key
```
Create a new file called `.env` in the project root folder and add:
GEMINI_API_KEY=your_gemini_api_key_here
To get a free API key: Go to [aistudio.google.com](https://aistudio.google.com) → click **"Get API Key"** → copy it
```
### Step 4: Run the App
```
streamlit run app.py
```
The app will open automatically in your browser at `http://localhost:8501`

---

## 🖥️ How to Use

1. **Pick a question** from the dropdown — HR or technical
2. **Type your answer** in the text box
3. **Click "Submit for Feedback"**
4. Zephyr analyses your answer and gives detailed AI feedback instantly

---

## 🧠 How It Works

**app.py** — The main entry point. Runs the Streamlit UI, handles user input, and calls the feedback engine.

**chatbot.py** — Connects to Google Gemini API. Sends your answer along with a coaching prompt and returns the AI's evaluation.

**feedback_engine.py** — Processes the raw AI response and formats it into structured, readable feedback for the user.

**question_bank.json** — Stores all interview questions in JSON format. Easy to extend by adding new questions to the file.

**resume_tips.py** — Standalone module that provides resume improvement tips — can be integrated into future versions as a separate tab.

---

## 📝 Environment Variables

Create a `.env` file in the root folder:
GEMINI_API_KEY=your_gemini_api_key_here

⚠️ Never share your API key publicly. The `.env` file is excluded from version control via `.gitignore`.

---

## 🚀 Future Enhancements

- [ ] Add more question categories (System Design, DSA, Behavioural)
- [ ] Score the answer out of 10 with breakdown
- [ ] Voice input support
- [ ] Save session history
- [ ] Deploy on Streamlit Cloud for public access
- [ ] Add difficulty levels (Fresher / Mid / Senior)

---

## 📜 License

MIT License — Free to use for educational and personal purposes.

---

## 👤 Author

**Geetesh Muralitharan**
- GitHub: [@geeteshkm](https://github.com/geeteshkm)
- Email: geeteshkm25@gmail.com
- LinkedIn: [Geetesh M](https://linkedin.com/in/geeteshkm)

---

⭐ If this project helped you, give it a star on GitHub!

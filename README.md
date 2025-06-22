# YourAIchat

YourAIchat is a responsive, modern web-based AI chatbot app built using Flask (Python) and Hugging Face's inference API. 
It features a sleek UI inspired by ChatGPT and DeepSeek, with support for dark/light themes, saved conversations, and mobile responsiveness.

## 🚀 Live Demo
https://youraichat-jx9v.onrender.com/



![Screenshot 2025-06-23 00 50 37](https://github.com/user-attachments/assets/9a10f775-a195-452b-bc4f-d86810aaa288)



##  Tech Stack

### Frontend

* **HTML5** – Markup for chat interface and layout
* **CSS3** – Custom styling, dark/light themes, mobile responsiveness
* **JavaScript (Vanilla)** –

  * Handles sending/receiving messages
  * Theme toggle
  * Save & load conversations

### Backend

* **Python 3.10+** – Core language
* **Flask** – Web server, API routing
* **huggingface\_hub** – For accessing Hugging Face inference models
* **dotenv** – For loading `.env` variables like API keys

### Deployment

* **Git + GitHub** – Version control
* **Render** – Hosting platform for the Flask server

---

## 📦 Features

* [x] Real-time AI responses via Hugging Face
* [x] ChatGPT-inspired UI (dark by default)
* [x] Light theme toggle
* [x] Save and view old chats
* [x] Start a new chat session anytime
* [x] Responsive layout for mobile and desktop
* [x] Stop AI response button

---

## ⚙️ Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/lathigaa/YourAIchat.git
cd YourAIchat
```

### 2. Set up environment

Create a `.env` file in the root directory:

```
HUG_API_KEY=your_huggingface_api_key_here
MODEL=your_preferred_model_id
```

Example model (free tier):

```
MODEL=HuggingFaceH4/zephyr-7b-beta
```

### 3. Install requirements

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install flask python-dotenv huggingface_hub
```

### 4. Run locally

```bash
python TextGenerator.py
```

Visit `http://localhost:5000` in your browser.

### 5. Deploy on Render

* Create a new **Web Service** on [Render](https://render.com/)
* Add environment variables:

  * `HUG_API_KEY`
  * `MODEL`
* Set Start Command:

```bash
python TextGenerator.py
```

* Render automatically detects the port from `os.environ["PORT"]`

---

## 📁 Project Structure

```
YourAIchat/
├── templates/
│   ├── index.html
│   └── style.css
├── TextGenerator.py
├── .gitignore
└── .env  (not pushed to GitHub)
```

---

## 🧠 Future Enhancements

* [ ] Add markdown & code block rendering
* [ ] Model selector UI
* [ ] Export chat as PDF/text
* [ ] Voice input & output (TTS/STT)


---

##  Acknowledgements

* Hugging Face for inference API
* ChatGPT & DeepSeek for UI inspiration
* Render for free hosting

---

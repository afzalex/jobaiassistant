# JobAIAssistant

**AI-powered automation tool that applies for jobs on your behalf with real-time visibility and control.**

---

## 🚀 Overview

JobAIAssistant is a smart job application automation tool designed for tech-savvy professionals and developers. It combines a web dashboard for configuring user profiles and preferences with a Playwright-powered local automation engine that interacts with job portals like LinkedIn and Naukri in a visible browser.

Users can watch applications being filled live, intervene when needed (e.g., login, CAPTCHA), and confirm before final submissions. It reduces the tedium of job hunting while ensuring full control and visibility.

---

## 🧩 Features

* Web dashboard for managing profiles and settings
* Real browser automation using Playwright (non-headless)
* Resume upload and auto form-filling
* Human-in-the-loop interaction for signups, logins, and CAPTCHAs
* Smart field mapping and job confidence scoring
* Email-based application support via Gmail API
* Modular, extensible, developer-friendly design

---

## ⚙️ Tech Stack

* **Frontend:** Next.js (React), Tailwind CSS
* **Backend:** FastAPI or Express (Node.js)
* **Automation:** Playwright (Python)
* **Database:** SQLite / PostgreSQL
* **Messaging:** WebSocket or polling
* **Email:** Gmail API with OAuth2

---

## 📁 Directory Structure

```
jobaiassistant/
├── automation/          # Browser automation scripts
├── dashboard/           # Web frontend (Next.js)
├── config/              # User profile config and constants
├── data/                # Logs, resumes, application status
├── server/              # Backend API server
├── shared/              # Common logic (form mapper, scorer)
└── main.py              # Automation entry point
```

---

## 🧪 Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/yourname/jobaiassistant.git
cd jobaiassistant
```

### 2. Install Python & Node.js dependencies

```bash
# Backend and automation
pip install -r requirements.txt

# Frontend
cd dashboard
npm install
```

### 3. Launch Components

```bash
# Run the web dashboard
cd dashboard
npm run dev

# Run the local automation bot
cd ..
python main.py
```

---

## ✨ Example Usage

1. Visit `http://localhost:3000` to configure your profile.
2. Click "Start Auto Apply" in the dashboard.
3. A browser opens, applies for jobs, and waits for you when needed.
4. Watch and assist the automation in real time.
5. Logs and screenshots are saved in `data/`.

---

## 🔐 Security

* No passwords are stored.
* OAuth2 used for Gmail.
* CAPTCHA and login are handled manually by user.
* All actions visible to the user.

---

## 📌 Roadmap

* ✅ Profile management via dashboard
* ✅ Playwright-based browser automation
* ⬜ Multi-resume support
* ⬜ Form classifier using AI
* ⬜ Telegram alerts for manual steps
* ⬜ Dockerized deployment

---

## 🤝 Contributing

Pull requests are welcome. Please open an issue first to discuss major changes.

---

## 📄 License

MIT License

---

**Made with ❤️ to save your time and sanity in job hunting.**

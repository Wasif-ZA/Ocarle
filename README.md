# 🧿 Ocarle – Voice-Powered Productivity Assistant

Ocarle is your personal AI-powered productivity assistant that listens to your voice, understands your goals, schedules your tasks, and reminds you when it matters — all while learning your routines. Inspired by the Oracle of Delphi, Ocarle brings clarity and structure to your modern life.

## 🎯 Vision

To build a voice-first productivity assistant that empowers individuals to manage their tasks with minimal friction and maximum adaptability. Ocarle aims to be context-aware, smart, and intuitive — delivering insightful nudges, smart scheduling, and voice-controlled task handling.

## 🚀 Features

- 📝 **Natural Language Task Input** via text or speech  
- 🔊 **Voice Commands** (powered by OpenAI Whisper)  
- 🎯 **Smart Task Prioritization & Suggestions**  
- ⏰ **Reminders, Snoozes & Notifications**  
- 🧠 **AI-Powered Conflict Detection**  
- 📆 **Google Calendar Sync**  
- 📈 **Habit Learning & Productivity Analytics**  
- 💬 **Conversational Chat UI** with emoji/voice input  
- 🔐 **Secure Auth with Supabase (Email/OAuth)**  
- 📱 **PWA Support & Mobile-Responsive UI**

## 🧱 Architecture Overview

| Layer              | Technology                          | Purpose                                  |
|-------------------|--------------------------------------|------------------------------------------|
| **Frontend**       | Next.js 15, Tailwind CSS, Framer Motion | Responsive, animated UI                |
| **Backend**        | Supabase, optional Spring Boot       | Auth, DB, logic, triggers                 |
| **AI / NLP**       | OpenAI API, Whisper, Google TTS      | Text/voice understanding & feedback      |
| **Scheduling**     | Supabase Edge Functions, cron jobs   | Timed reminders and task triggers        |
| **Integrations**   | Google Calendar API, Telegram API    | Calendar syncing, alerts, notifications  |
| **Optional**       | React Native / Expo                  | Full native mobile support (future)      |

## 📁 Folder Structure

```
/src
  /components         # Reusable UI elements (TaskCard, Sidebar, etc.)
  /pages              # App routes and views
  /hooks              # Custom React hooks
  /lib                # Utility/helper functions
  /utils              # Logic functions (date parsing, priority checks)
  /styles             # Tailwind and global CSS
```

## 📅 Roadmap (6-Month Plan)

| Phase                    | Timeline     | Key Milestones                                           |
|--------------------------|--------------|----------------------------------------------------------|
| **1. MVP Core**          | Weeks 1–4     | Task dashboard, Supabase DB, manual reminders            |
| **2. Assistant Logic**   | Weeks 5–8     | NLP parser, recurring task handling, conflict detection  |
| **3. Voice & Mobility**  | Weeks 9–12    | Whisper API, TTS feedback, PWA/mobile layout             |
| **4. Personalization**   | Weeks 13–16   | Habit learning, analytics dashboard                      |
| **5. Chat UI**           | Weeks 17–20   | Conversational interface, emoji/voice input              |
| **6. Polish & Deploy**   | Weeks 21–24   | Google Calendar sync, bug fixes, launch-ready polish     |

## 🧪 Testing Approach

- ✅ **Alpha Testing** for functional units (task creation, reminders)  
- ✅ **Beta Testing** for usability and feedback from early users  
- 📉 **Performance Testing**: 1,000+ concurrent reminders  
- 🎙️ **Voice Input Accuracy**: Lighting, noise, accent testing  
- 🔁 **Reminder Reliability**: Edge trigger and delay stress tests

## 📊 Analytics

Tracked metrics:  
- ✅ Task completion rate  
- ⏱️ Average time to completion  
- 💤 Frequency of snoozed tasks  
- 🧠 Most productive hours  
- 📈 Weekly & Monthly task trends  

## 🔐 Authentication & Security

- Supabase Auth (Email + OAuth)  
- Password reset + session expiration  
- Environment variables stored in `.env.local`  
- Role-based access planned for admin dashboards  

## 🧠 Future Enhancements

- 🤖 AI-powered daily plans based on habits and deadlines  
- 🔁 Context-aware auto-rescheduling  
- 🧩 Plugin API for third-party integrations (Notion, Trello)  
- 🌐 Chrome Extension for instant task capture  
- 📱 Full native mobile app (React Native or Flutter)  

## 🛠️ Setup Instructions

1. **Clone the repo**
   ```bash
   git clone https://github.com/Wasif-ZA/Ocarle.git
   cd Ocarle
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   - Copy `.env.example` to `.env.local` and add:
     ```
     NEXT_PUBLIC_SUPABASE_URL=
     NEXT_PUBLIC_SUPABASE_ANON_KEY=
     OPENAI_API_KEY=
     GOOGLE_CALENDAR_CLIENT_ID=
     ```

4. **Run the dev server**
   ```bash
   npm run dev
   ```

5. **View the app**
   - Open your browser to [http://localhost:3000](http://localhost:3000)

## 📚 Resources

- [OpenAI API](https://platform.openai.com/)  
- [Supabase Docs](https://supabase.com/docs)  
- [Whisper (Speech-to-Text)](https://openai.com/research/whisper)  
- [Google Calendar API](https://developers.google.com/calendar)  

## 👤 Author

**Wasif Zaman**  
[🌐 Portfolio](https://wasifzaman-io.vercel.app)  
[🐙 GitHub](https://github.com/Wasif-ZA)  
[💼 LinkedIn](https://www.linkedin.com/in/wasif-zaman-4228b5245/)

---

> “A modern Oracle — not of prophecy, but of productivity.”

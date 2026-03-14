# 🚀 TaskFlow Elite OS (v4.0)

**TaskFlow Elite OS** is the ultimate productivity and task management application. The uniqueness of this project is that this complete, massive functionality works **entirely without servers, without frameworks, and without third-party libraries**, fitting into just **a single `index.html` file**.

## ✨ Key Features

- 🌍 **Multilingual Out of the Box (i18n):** Supports 8 languages (English, Russian, German, French, Spanish, Italian, Ukrainian, and Chinese). Prompted on first launch.
- 🗂 **Workspaces:** Separate your "Work", "Study", and "Personal" tasks into isolated environments.
- 📋 **Kanban & Lists:** Toggle between a classic list view and a Kanban board with smooth **Drag & Drop**.
- 🍅 **Floating Pomodoro Timer:** A movable timer for deep work. Earn XP for completing focus sessions.
- 🎮 **Gamification:** Earn XP, level up, and maintain a daily login "Streak" (🔥).
- 🏆 **Hall of Fame (Achievements):** Achievement system with popping toasts and fanfares (audio generated via `Web Audio API`).
- 📊 **Analytics Dashboard:** Built-in analytics with custom-drawn SVG charts for your task completion statistics.
- 📅 **Calendar View:** A convenient monthly grid that automatically plots task deadlines.
- 📱 **PWA (Installable):** TaskFlow dynamically generates a `manifest.json` and a Service Worker right in the browser, allowing you to install it on your phone or PC via the "Install App" button without needing a backend.
- 💌 **Telegram Notifications:** Built-in push notifications for burning deadlines directly to your Telegram! (See "Telegram Setup" below).

## 🛠 Tech Stack

- **HTML5 & CSS3** (Grid, Flexbox, Glassmorphism, CSS Variables)
- **Vanilla JavaScript** (ES6+)
- **DOM API** (Drag and Drop, LocalStorage, Web Audio API)
- ❌ No React, Vue, Webpack, or Node.js. **Zero dependencies.**

## 🚀 How to Run

You don't need to install `npm` packages or spin up a local server.
1. Download or clone this repository.
2. Just open the `index.html` file in any modern browser.
3. Enjoy!

> 💡 **Resetting Data:** If you want to wipe all your progress, tasks, and choose the language again, open Developer Tools (F12) and type `localStorage.clear()` in the console, then refresh the page.

## 🤖 Telegram Reminders Setup

The app can send you push notifications about burning deadlines directly to Telegram (it checks your tasks every minute).

To make it work:
1. Create a bot in Telegram via [@BotFather](https://t.me/BotFather) and copy its Token.
2. Find out your personal `chat_id` (e.g., via the @userinfobot).
3. Open TaskFlow in your browser, press `F12` (Developer Console), and enter these two commands:
   ```javascript
   localStorage.setItem('TF_TG_BOT', 'YOUR_BOT_TOKEN_HERE');
   localStorage.setItem('TF_TG_CHAT', 'YOUR_CHAT_ID_HERE');
   ```
4. Refresh the page. Now the bot will ping you directly in Telegram if a task's deadline matches the current day!

## 📜 License

MIT License. Made with love for clean code.

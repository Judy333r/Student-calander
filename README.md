# School E-Calendar

A cute, customizable school planner that runs entirely in the browser. No backend, no build step, no dependencies. Built with plain HTML, CSS and JavaScript so it works on GitHub Pages.

## Features

- Monthly calendar with today highlighted and indicators for exams, tasks and reminders
- Daily page with subjects, exams, school work, reminders and auto-saving notes
- Weekly school timetable (add, edit, delete, reorder)
- Automatic subject comparison between a day and the next day:
  - 🟢 ↑ Extra Subjects (added tomorrow)
  - 🔴 ↓ Deducted Subjects (not scheduled tomorrow)
- 14 themes plus a custom color picker
- English and Arabic, with full RTL layout and Arabic month/day names
- Everything saved in your browser's localStorage
- Responsive for phone, tablet, laptop and desktop

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page shell: loads fonts, styles and the script |
| `style.css` | Layout, theme variables, RTL-safe styling |
| `script.js` | All app logic, translations and pages |

All three files must stay in the same folder.

## Deploy to GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `style.css`, `script.js` and `README.md` to the root of the repository.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set the source to **Deploy from a branch**.
5. Choose the `main` branch and the `/ (root)` folder, then save.
6. After a minute or two, your site is live at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

## Run locally

Double-click `index.html` to open it in a browser. No server is needed.

## How it works

`index.html` contains only an empty `<div id="app">`. `script.js` builds every page into it (home, calendar, day, schedule, themes, settings) and re-renders when you navigate or change language or theme.

## Using the planner

- **Name:** type it on the home page. The title becomes "Name's Calendar".
- **Timetable:** open **Schedule** and add subjects to each weekday. The calendar uses it automatically.
- **Daily page:** tap any date to add exams, tasks, reminders and notes.
- **Subject changes:** on a daily page, the green and red lines show what changes tomorrow. Tap them for details.
- **Themes:** tap the big circle on the home page, or open **Themes**. Changing theme never deletes data.
- **Language:** switch in **Settings**. Your own text is never translated.
- **Reset:** **Settings → Reset all data** asks for confirmation first.

## Data and privacy

All data stays in your browser on your device. Nothing is sent anywhere. Clearing your browser data, or using a different browser or device, means starting fresh. Private browsing windows may not keep data after you close them.

## Troubleshooting

- **Blank page:** make sure all three files are in the same folder and named exactly `index.html`, `style.css` and `script.js`.
- **Changes not showing on GitHub Pages:** wait a minute, then hard refresh (Ctrl+Shift+R, or Cmd+Shift+R on Mac).
- **Data missing:** localStorage is per browser and per site address, so a new URL or browser won't have your old data.
- **Fonts look different offline:** fonts load from Google Fonts. Without internet, the page falls back to your system fonts.

## Browser support

Any modern browser (current Chrome, Safari, Firefox, Edge), including iPhone and iPad Safari.

# QuickNotes

QuickNotes is a small note-taking web app for capturing quick thoughts before they slip away. You type a note, pick a category (Personal, Work or Study), and it appears as a colour-coded card. Everything is saved in your browser, so your notes are still there when you come back. It is built with plain HTML, CSS and JavaScript, with no frameworks.

## Features

- Add notes with a category: Personal, Work or Study
- Each note shows its text, a category label, the date and time it was created, and a Delete button
- Colour-coded cards, with a different left border and label colour for each category
- Friendly validation: empty notes and notes over 200 characters show an error message
- Live search that filters notes as you type, ignoring upper and lower case
- A note count that reads correctly for zero, one and many notes
- Notes are saved with `localStorage`, so they survive a page refresh
- "Clear all" button that asks for confirmation first (bonus)
- Responsive layout that stacks the form on small screens

## How to run it locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/quicknotes-app.git
   ```
2. Open the `quicknotes-app` folder in VS Code.
3. Right-click `index.html` and choose **Open with Live Server** (or just double-click `index.html` to open it in your browser).

## What I learned

- How to rebuild a whole list from one array with `createElement` and `textContent`. This is safer than `innerHTML`, because user text can never be run as code.
- How to keep data between visits using `localStorage`, with `JSON.stringify` to save and `JSON.parse` to load, plus a fallback for when nothing (or something broken) is saved.
- How Flexbox and a `@media (max-width: 600px)` rule make one layout work on both desktop and phone.
- How to plan a project in small steps and make a commit after each one, so the Git history tells the story of how the app was built.

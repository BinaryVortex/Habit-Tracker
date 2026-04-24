# Habit Tracker

A simple, clean habit tracker built with HTML, CSS and JavaScript — perfect for tracking daily habits, marking progress, and exporting/importing your data.

![App Screenshot](./Screenshot%202024-07-11%20040833.png)

## Live Preview
Open `index.html` in your browser to try the app locally.

## Features
- Add, edit and delete habits
- Mark habits as completed (stores completion date)
- Filter to show/hide completed habits
- Clear all completed habits
- Export habits as CSV
- Import habits from a JSON file
- Data persisted in localStorage (no backend required)

## How it works
- Habits are stored as an array of objects in localStorage. Each habit object contains:
  - id: unique numeric id generated with Date.now()
  - name: name of the habit
  - completed: boolean
  - datesCompleted: array of completion dates (strings)
- The UI updates dynamically when you add, toggle, edit or remove habits.

## Usage
1. Open `index.html` in your browser.
2. Type a habit into the input and click "Add Habit" (or press Enter).
3. Click the checkbox to mark a habit as completed. The date will be recorded.
4. Use "Show Completed" to toggle visibility of completed items.
5. Click "Clear Completed" to remove completed habits.
6. Export to CSV with the "Export Habits" button. Import JSON using the hidden file input (click the import area from the DOM or modify the UI to reveal it).

## Run locally
1. Clone the repo:

```bash
git clone https://github.com/BinaryVortex/Habit-Tracker.git
cd Habit-Tracker
```

2. Open `index.html` in your browser.

Optional: Use a simple local server (recommended for some browsers):

```bash
# Python 3
python -m http.server 8000
# then visit http://localhost:8000
```

## File structure
- index.html — main HTML file
- style.css — styling and layout
- script.js — application logic
- Screenshot 2024-07-11 040833.png — app screenshot

## Contributing
Contributions are welcome — open an issue or submit a pull request. Suggestions:
- Add categories or priorities to habits
- Add streak counters and charts
- Improve import UI and file format validation

## License
This project is open source — feel free to reuse and modify.

---

Made with ❤️ by BinaryVortex

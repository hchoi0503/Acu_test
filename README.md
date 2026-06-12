# Acupuncture Quiz

A clean, offline-capable interactive quiz application for acupuncture board exam preparation with a smart mastery system.

## Features

- **1210 high-quality questions** across multiple acupuncture topics
- **Smart Mastery System**:
  - Questions you get wrong are tracked as "Missed"
  - Missed questions stay in rotation until you answer them correctly **2 consecutive times**
  - Option to manually mark questions as "Mastered"
- **Flexible Quiz Length**: Choose between 10-question or 20-question quizzes
- **Intelligent Question Selection**:
  - Prioritizes missed questions (3–4 in a 20-question quiz)
  - Includes a healthy number of never-seen questions
- **Detailed Review Screen**: Shows the actual answer text (not just A/B/C) after each quiz
- **Progress Persistence**: Your progress is saved automatically in the browser using `localStorage`
- **Mobile Friendly**: Fully responsive design

## File Structure

```
.
├── index.html       # Main quiz application
├── questions.json   # Question database (1210 questions)
└── README.md
```

## How to Run Locally

### Option 1: Using VS Code Live Server (Recommended)

1. Open the folder in Visual Studio Code
2. Right-click on `index.html`
3. Select **"Open with Live Server"**

### Option 2: Using Python

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

### Option 3: Using Node.js

```bash
npx serve .
```

## Deploying to GitHub Pages

1. Push both `index.html` and `questions.json` to your GitHub repository.
2. Go to your repository **Settings → Pages**.
3. Under **Build and deployment**, set:
   - Source: **Deploy from a branch**
   - Branch: `main` (or `master`)
4. Save. Your quiz will be live at:

   `https://<your-username>.github.io/<repository-name>/`

## Notes

- This is a **static website** — no backend or database required.
- All progress is stored locally in your browser (`localStorage`). It will not sync across devices.
- For best results, always serve the files using a local server or GitHub Pages (do **not** open `index.html` by double-clicking it directly).

## Credits

Built for acupuncture students preparing for board exams. Questions are based on standard acupuncture curriculum and clinical knowledge.

---

Enjoy studying!

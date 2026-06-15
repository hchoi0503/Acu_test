# Acupuncture Quiz

A modern, feature-rich web app for preparing for the NCCAOM acupuncture board exams. Built with a smart mastery system, domain-based filtering, exam simulation, and personal notes.

## Features

- **1210 High-Quality Questions** across all 4 NCCAOM domains
- **Smart Mastery System**
  - Tracks correct streaks and miss counts
  - Prioritizes questions you struggle with the most
  - Questions move to "Mastered" after 2 consecutive correct answers
- **Domain Performance Tracking**
  - See your mastery percentage per domain with progress bars
  - Reset progress for individual domains
- **Flexible Study Modes**
  - Quick quizzes (10 or 20 questions)
  - Focus on your weakest domains with one click
  - Full Practice Exam mode with real NCCAOM domain weighting (Domain III = 40%)
- **Domain Filtering**
  - Study specific domains or any combination
- **Review & Reflection Tools**
  - Flag difficult questions
  - Add personal notes to any question
- **Progress Insights**
  - Recent progress trends shown on the home screen
- **Progressive Web App (PWA)**
  - Installable on phones and tablets
  - Works offline after first load
- **Mobile Optimized**
  - Comfortable touch targets and responsive layout

## File Structure

```
.
├── index.html                          # Main application
├── questions_refined_4_domains.json    # Question database (1210 questions)
├── manifest.json                       # PWA manifest
├── service-worker.js                   # Service worker for offline support
└── README.md
```

## How to Run Locally

### Option 1: VS Code Live Server (Recommended)

1. Open the project folder in Visual Studio Code
2. Right-click on `index.html`
3. Select **"Open with Live Server"**

### Option 2: Python HTTP Server

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

### Option 3: Node.js

```bash
npx serve .
```

## Deploying to GitHub Pages

1. Push all files to your GitHub repository.
2. Go to **Settings → Pages**.
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: `main` (or `master`)
4. Save. Your app will be live at:

   `https://<your-username>.github.io/<repository-name>/`

After deployment, users can install the app on their phones via the browser’s “Add to Home Screen” option.

## Important Notes

- All progress (mastery, notes, flags) is stored in your browser’s `localStorage`.
- Progress **does not sync** across devices.
- The app works fully offline after the first visit (thanks to the service worker).
- For best icon appearance when installing as a PWA, add `icon-192.png` and `icon-512.png` to the project root (optional).

## Credits

Built for acupuncture students preparing for the NCCAOM board exams. Questions are based on standard acupuncture curriculum and clinical knowledge.

---

Enjoy your studies!

# AptiAI 50+ — AI-Powered Aptitude Assessment & Dataset Engine

A single-page React web application designed for structured aptitude evaluation, timed exam simulation, interactive practice, and question bank management[cite: 1]. It includes a built-in dataset of 50+ questions (56 questions across 6 domains) tailored for technical screenings, entrance tests, and placement assessments[cite: 1, 6, 8].

**Student Details:** Yashowardhan Shete | Roll No: 50 | Class: AIA6 (Artificial Intelligence & Automation) | Academic Year: 2025–2026[cite: 1]

---

## Features

* **Analytics Dashboard:** Tracks quizzes completed, average accuracy percentage, best test score, and total questions answered[cite: 2, 8]. Displays recent test attempts and quick-access bookmarked questions[cite: 2, 8].
* **AI Quiz Generator Configurator:** Lets users choose between **Exam Simulation** (timed test with deferred solutions) and **Interactive Practice** (untimed with instant feedback and hints)[cite: 2, 7, 11]. Supports filtering by domain category, difficulty level (`All`, `Easy`, `Medium`, `Hard`), question count (`5–30`), and time limits (`No Timer`, `5`, `10`, `15`, or `20` minutes)[cite: 2, 7, 11].
* **Live Quiz Player:** Features a countdown timer in exam mode, domain and difficulty badges, option selection, question bookmarking, a **Hint / Key Formula** modal, and instant explanations in practice mode[cite: 2, 5, 11].
* **Performance Scorecard & Solution Key:** Shows final accuracy, correct and incorrect counts, time spent, and a step-by-step solution breakdown for every question[cite: 3, 4, 11].
* **Question Bank Explorer & Dataset Portability:** Supports keyword search, category and difficulty filtering, adding custom questions, and bulk JSON import/export[cite: 3, 6, 11]. Saves dataset changes, bookmarks, and attempt history in browser `localStorage`[cite: 2, 9].
* **Dark & Light Theme Support:** Includes a theme toggle in the top navigation bar[cite: 2, 9, 11].

---

## Built-In Dataset Domains (56 Questions)

| Domain Category | Count | Key Topics Covered |
| :--- | :---: | :--- |
| **Quantitative Aptitude** | 12[cite: 1] | Work & Time, Profit & Loss, SI/CI, Speed & Distance, Ratio & Proportion, Averages, Permutation & Combination, Probability[cite: 1, 9] |
| **Logical Reasoning** | 10[cite: 1] | Series Completion, Blood Relations, Coding-Decoding, Syllogisms, Seating Arrangement, Statement & Assumption[cite: 1, 9] |
| **Verbal Ability** | 10[cite: 1] | Synonyms & Antonyms, Error Spotting, Sentence Improvement, Idioms & Phrases, Reading Comprehension[cite: 1, 9] |
| **Data Interpretation** | 8[cite: 1] | Table Data, Pie Charts, Bar Graphs, Data Sufficiency, Weighted Averages[cite: 1, 9] |
| **Computer & Coding Concepts** | 10[cite: 1] | Time Complexity, Data Structures (LIFO, Balanced BST/AVL), Python & JS Outputs, OOPs, SQL[cite: 1, 9] |
| **Spatial & Abstract Reasoning** | 6[cite: 1] | Mirror Images, Rotational Patterns, Matrix Reasoning, Triangle Counting, Painted Cubes[cite: 1, 9] |

---

## Project Structure

```text
aptiai-50-project/
├── index.html
├── package.json
├── postcss.config.js
├── tailwind.config.js
├── tsconfig.json
├── vite.config.ts
└── src/
    ├── App.tsx
    ├── index.css
    ├── main.tsx
    ├── types/
    │   └── aptitude.ts
    ├── data/
    │   └── builtinDataset.ts
    └── components/
        ├── Navbar.tsx
        ├── DashboardView.tsx
        ├── GeneratorView.tsx
        ├── QuizPlayerView.tsx
        ├── ResultsView.tsx
        └── QuestionBankView.tsx

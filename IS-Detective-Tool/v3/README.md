# IS Detective Tool — CPSC 201

Standalone GitHub Pages site for Pizza Shop Enterprise.

## What's included
- Home page: student name, investigator role, department, total score.
- Problem Analysis Card: 4 guided practice cases and 6 independent challenges (Cases 5–10), maximum three submissions per challenge; 10 points for first correct attempt, 3 for second, 0 for third. Total possible: 60.
- Problem Evidence Card: displays evidence for the **department and role chosen on the home page**, with a case selector (Cases 5–10), question recording, selected evidence sharing, and exportable log.
- Progress is stored in the browser using localStorage; nothing is sent to a server.

## Publish
1. Create a public GitHub repository.
2. Upload `index.html`, `style.css`, and `app.js` to the repository root.
3. In Settings → Pages, choose Deploy from a branch → main → /(root).
4. Open `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.

## Classroom usage and privacy
Students choose their role and department on the home page, then lock their profile before entering either card. The normal interface prevents role or department changes after locking. Starting over requires two confirmations and erases all locally saved scores, answers, and evidence logs on that device. Department representatives use the evidence card and share relevant facts verbally when asked. Investigators use the analysis card to submit diagnoses. The evidence cards are **not technically confidential**: this is a static site with no login or backend. The profile lock is a user-interface restriction, **not secure access control**: students with technical knowledge can inspect public source files or alter browser storage. Do not use this design for confidential data. Data and logs are stored separately on each browser/device and are not synchronized.

The six challenges use the same four-answer structure and three-attempt scoring. Four practice cases are unchanged from the previous release.

## Reset and start again
The home page displays **Reset & start again** before and after profile locking. If a student chose the wrong name, role, or department, they can reset after confirming. This clears this browser's local IS Detective profile, scores, answers, and evidence-sharing logs, then returns to the registration page. It does not affect other devices.

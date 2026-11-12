# IS Detective — GitHub Pages V5

## Features
- Standalone site with home-page student registration, role, department, profile lock, reset, and cumulative score.
- Four guided practice cases and six scored challenges. Affected components vary across People, Process, Data, and Technology.
- Every challenge has case-specific evidence for all nine departments, with shareable IDs such as `HUM-05-1`. The Evidence Card is filtered to the student's locked department.
- Department representatives receive verbal questions and log the facts they share, with copy/download options.
- Investigators enter **at least two valid evidence IDs from two distinct departments** plus at least 30 characters of reasoning before they can submit the four-part diagnosis.
- First correct attempt earns 10, second earns 3, third earns 0. A third attempt locks the challenge, correct or incorrect. Maximum total score: 60.

## Deploy to GitHub Pages
Upload `index.html`, `style.css`, and `app.js` to the repository root. In Settings → Pages, select Deploy from a branch, `main`, `/ (root)`.

## Important limitations
This is a **static classroom exercise**, not secure role-based access control. The locked department only limits the normal interface. All evidence is present in public site files. Students can inspect source code or browser storage. Evidence IDs validate against the built-in case catalog but **cannot prove an actual conversation occurred**. Students must exchange evidence in person and instructors should check logs/notes. Browser progress is local and does not synchronize across students. Reset clears this device's saved data. No backend or student-data upload.

## V5 change
Storage uses a new versioned key to prevent previous-version answer choices from mismatching the revised challenge choices. Students will register again after upgrading.

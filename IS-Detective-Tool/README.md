# IS Detective Tool — CPSC 201

Standalone, static GitHub Pages classroom tool with two options:

- **Problem Analysis Card**: Four guided training cases and a Case 5 independent challenge, maximum three submissions, scored 10 / 3 / 0.
- **Problem Evidence Card**: Nine department evidence sets, representative details, question recording, evidence selection, and a sharing log with TXT export.

## Publish on GitHub Pages

1. Create a new public GitHub repository, e.g. `is-detective`.
2. Upload `index.html`, `style.css`, and `app.js` to the repository root (not the ZIP file).
3. In repository **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
4. Once deployed, open `https://YOUR-USERNAME.github.io/is-detective/`.

No build step, server, external libraries, or account required.

## Classroom instructions

- Investigators use the Problem Analysis Card.
- Other students act as representatives of departments and open the Problem Evidence Card for their assigned department.
- Investigators ask representatives questions **face-to-face**. Representatives share relevant evidence and record each exchange.
- Investigators use their findings to diagnose Case 5.

## Important limitations

- All evidence is shipped in public client-side JavaScript. Department confidentiality is a **classroom convention**, not secure access control.
- The tool uses browser `localStorage` to retain progress on the **same browser and device**; there is no cross-device sync, student authentication, or instructor dashboard.
- Evidence logs are stored locally. Download logs to collect submissions.
- The Problem Analysis Card is intentionally designed for the People Investigator in Sales; changing the profile does not change its five cases.
- There is no fourth attempt after three submissions. The last case is Case 5, so navigation ends there.
- The Case 5 scenario is deliberately shortened to avoid revealing the investigation's key evidence before students contact departments.

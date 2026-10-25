# Resume to Readiness — updated prototype

## What's included
- Official "Resume to Readiness" branding and custom SVG logo.
- Responsive dashboard and navigation.
- Resume Lab target role, industry, location, current/target salary, goal period, background, and weekly study hours.
- Initial rule-based resume text scan with evidence-aware notes for skills, projects, experience, education, achievement signals, and readability signals.
- Roadmap task list.
- Cost Points levels: Starter (0+), Master (100+), Pro (300+), Pro Max (600+).
- Evidence submission, local demo verification/rejection, and activity history.
- Weekly points/hours graph and summary.
- Browser local storage for prototype data.

## Run locally
1. Extract the ZIP.
2. Open the extracted `Resume_to_Readiness` folder in VS Code.
3. In VS Code, select Terminal → New Terminal.
4. Run `python -m http.server 5500` (Windows alternative: `py -m http.server 5500`).
5. Open `http://localhost:5500` in your browser.
6. Keep the terminal running while you use the site.

You can also use the VS Code Live Server extension and open `index.html` with Live Server.

## Deploy for a public demo (GitHub Pages)
1. Create/sign in to a GitHub account and create a new public repository, e.g. `resume-to-readiness`.
2. Upload `index.html`, `styles.css`, `app.js`, and the `assets` folder to the repository root (you may upload README too).
3. Open repository Settings → Pages.
4. Under Build and deployment, select Deploy from a branch.
5. Choose branch `main` and folder `/(root)`, then Save.
6. Wait for the Pages URL to appear on the Pages screen and open it.
7. Test the published URL on both desktop and mobile.

Alternative: Netlify Drop — open Netlify, sign in if needed, and drag the extracted project folder (or a ZIP containing the files at its root) into the manual deploy area.

## Important limitations — read before presenting as production-ready
- This is a front-end prototype. User data is saved in the current browser's local storage; it is not a secure multi-user database and does not sync between devices.
- The "Demo verify" button is only for testing the flow. It does not prove that submitted work is genuine. Real verification requires authenticated reviewer accounts, evidence storage, review permissions, and an audit log on a server.
- Resume analysis is a transparent, simple keyword/section heuristic. It is not validated, does not extract PDF/DOCX files, cannot verify truth, cannot guarantee ATS compatibility, employability, salary, or career outcomes.
- In this version, TXT resume files can be loaded; PDF/DOCX text can be pasted manually. Do not upload sensitive/confidential information.
- Salary is a user-entered goal only; the prototype does not estimate or validate salary ranges.
- There is no real login, AI/LLM API, shared social network, or server-backed A* route planner yet.
- Before handling real people’s resumes, add secure authentication, HTTPS, server-side access controls, data retention/deletion controls, secure file handling, a real database, backups, and privacy/security review.

## Files
- `index.html`: page structure
- `styles.css`: responsive styling
- `app.js`: local prototype logic
- `assets/logo.svg`: official project mark

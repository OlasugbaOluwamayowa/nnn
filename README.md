# NOVEMBER — Personal NNN Progress Tracker

A simple, personal November challenge tracker. There is **no login, username, or password system**. A participant enters a display name and tracks progress in the browser they are using.

## Run the website locally
1. Install Node.js (LTS).
2. Extract this ZIP and open the `NOVEMBER` folder in VS Code.
3. Open Terminal in that folder.
4. Run `npm install`.
5. Run `npm run dev`.
6. Open the localhost address Vite prints (normally `http://localhost:5173`).

## Deploy it
This is a Vite project. When importing the project into a hosting provider such as Vercel, use:
- Framework preset: **Vite**
- Build command: `npm run build`
- Output directory: `dist`

The repository should contain the contents of this project folder (including `package.json`), not just the ZIP file.

## Included
- Responsive personal dashboard
- Display name only — no sign-up or login flow
- Daily success / setback check-ins
- Confirmation before changing an existing check-in
- November calendar with status colours
- Successful days, setbacks, streaks and completion percentage
- Daily activity chart
- PDF, CSV and JSON progress exports
- Local browser storage and delete-data control

## Privacy and storage — please read
The display name and progress are saved in the browser's `localStorage` on the current device. The app does not upload these records to a NOVEMBER server. There are no accounts and no cross-device synchronisation.

This is **not** verified zero-knowledge encryption. Anyone who can use the same browser profile may be able to view the saved data. Clearing browser data can erase it. Avoid using a shared device if the records are private, and export a backup if you want to keep a copy.

## Technology
React, TypeScript, Vite, Recharts, Lucide icons and jsPDF.

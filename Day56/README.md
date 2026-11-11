# LaunchPath AI — Day 6 MVP update

Day 6 adds aptitude and coding practice to the existing standalone LaunchPath AI prototype while preserving its roadmap, learning library and curated tutor.

## Run locally

No package installation, API key, database or build step is required.

1. Download or clone the project folder.
2. Open `index.html` in a modern browser (Chrome, Edge or Firefox).
3. Use the **Aptitude practice** tab to select a topic/difficulty, answer a question and click **Check answer**.
4. Use **Coding & DSA** to read a problem, reveal hints, inspect the Java reference solution and mark it as self-practiced.
5. Refresh the page and confirm that attempts and coding progress remain available in the same browser.

## Day 6 features

- Curated quantitative aptitude and logical reasoning question bank.
- Answer validation with worked explanation and learning tip.
- Attempt history, overall accuracy and topic-wise accuracy.
- Coding fundamentals and DSA problem cards with constraints and examples.
- Progressive hints, Java reference solutions, time/space complexity and edge cases.
- Local browser persistence with a delete-all-data control.
- Clear disclosure that this is not an online coding judge and does not execute arbitrary code.
- Required AB Talks challenge footer.

## Storage and limitations

Roadmap progress, notes, aptitude attempts and coding self-practice status are stored in browser `localStorage` on the current device/browser. Data is not synced across devices and clearing browser storage removes it. The coding section provides reference material and self-reported completion only; it does not run code or verify hidden test cases.

## Deployment

This is a static HTML application and can be deployed on a free static hosting tier such as GitHub Pages or Netlify Drop. No environment variables or secrets are required. Deployment and live-site verification must be completed from the user's GitHub/hosting account.

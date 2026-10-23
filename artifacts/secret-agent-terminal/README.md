# Secret Agent Hacker Terminal & Mini-Game

A beginner-friendly, fictional spy-console demo for a college AI Coding Lab. It is made with browser-native HTML, CSS, and JavaScript in one file: `index.html`. It does not connect to networks, scan real devices, or perform real hacking.

## Features

- A responsive dark terminal with animated Matrix-style rain.
- Fictional terminal activity and an explicitly simulated scan with progress feedback.
- Interactive controls for trying the demo.
- A cipher-decoding mini-game.
- Three in-page `console.assert()` checks for a normal, zero/empty, and invalid input.
- Reduced-motion support and no external services or APIs.

## Usage

1. Open `index.html` in a modern browser. No installation or account is needed.
2. Use the on-screen controls to start the simulated activity and follow the cipher prompt.
3. The scan is visual feedback only; it never contacts a host or tests a real system.

## Testing

1. Open `index.html` in Chrome, Firefox, or another modern browser.
2. Open the browser developer tools (`F12` or `Ctrl+Shift+J` on Windows/Linux; `Option+Command+J` on macOS) and select **Console**.
3. Reload the page. The three assertions run automatically. Passing assertions stay quiet; a failed assertion appears in red.
4. Try the controls and cipher game, and check that the simulated scan reaches completion and the page remains usable at a narrow phone width.

## Debugging exercise: introduce, diagnose, and restore a small bug

1. Save a copy of `index.html` or create a Replit checkpoint so you can restore the working version.
2. In the `decodeCaesar` function in `index.html`, temporarily change the letter-shift expression so it adds the shift instead of subtracting it.
3. Save and reload the page. Open the browser Console and find the failed “Normal cipher input should decode” assertion. The cipher will also stop accepting the intended answer.
4. Ask an AI coding assistant: “The normal-input console assertion for `decodeCaesar` is failing. Explain why, then fix the letter shift so each character moves backward by the requested number.”
5. Review the suggested edit, apply it, and reload the page. Check that the assertion failure is gone and the cipher accepts the decoded message. If you want to return to the original working file, undo the edit or restore the checkpoint you made in step 1.

This exercise creates a visible test failure, not a security vulnerability. Do not change the simulation to contact or probe real systems.

## Publish with GitHub Pages

This project is static, so you can host it with GitHub Pages without a server:

1. Create a GitHub repository and add `index.html` and this `README.md` to the repository's top level.
2. Open the repository's **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select the `main` branch and the `/ (root)` folder, then save.
4. Wait for GitHub Pages to finish publishing and use the URL shown in the Pages settings.

These are publishing instructions only; the project has not been deployed from this workspace.

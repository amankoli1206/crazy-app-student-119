# 🕵️ Secret Agent Terminal & Mini-Game

A retro-futuristic, cyberpunk spy-console and interactive cipher mini-game designed for simulated security labs, AI pair-programming demos, and coding education.

---

## 🌟 Overview

The **Secret Agent Terminal** simulates a covert operative's workstation complete with animated digital rain, diagnostic scanner sequences, fictional system commands, and an interactive Caesar cipher decryption puzzle.

> **Note:** This is purely a fictional simulation built for educational and demonstration purposes. It does not connect to real external networks or perform real security testing.

---

## ✨ Features

- **Matrix-style Digital Rain**: Canvas-rendered ambient rain animation with responsive frame rates.
- **Operative Console UI**: Authentically styled retro-terminal aesthetic with scanline effects and dark neon palette.
- **Diagnostic System Scanner**: Animated scan progression with live simulated terminal logging.
- **Cipher Decryption Mini-Game**: Interactive puzzle challenge testing Caesar cipher decoding skills.
- **Console Self-Tests**: Built-in `console.assert()` test suite validating normal, empty, and invalid inputs.
- **Accessibility Friendly**: Includes `prefers-reduced-motion` detection and fully responsive layout.

---

## 🚀 Quick Start

### Option 1: Standalone Browser (Zero Install)
You can run the web terminal directly without installing any dependencies:
1. Navigate to [`artifacts/secret-agent-terminal/index.html`](file:///Users/amankoli/Desktop/Secret-Agent-Terminal/artifacts/secret-agent-terminal/index.html).
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge).

### Option 2: Full Monorepo Workspace (pnpm)
If working within the monorepo:

```bash
# Install dependencies
pnpm install

# Run typechecks across workspace
pnpm run typecheck

# Build workspace packages
pnpm run build
```

---

## 📁 Repository Structure

```text
Secret-Agent-Terminal/
├── artifacts/
│   ├── secret-agent-terminal/    # Main spy terminal application & client UI
│   ├── api-server/               # Express backend API service
│   └── mockup-sandbox/           # UI component staging & sandbox
├── lib/
│   ├── api-client-react/         # React query hooks generated for API client
│   ├── api-spec/                 # OpenAPI specification & codegen setup
│   ├── api-zod/                  # Zod validation schemas
│   └── db/                       # PostgreSQL schema & Drizzle ORM config
├── scripts/                      # Workspace utility scripts
├── package.json                  # Root monorepo configuration
└── pnpm-workspace.yaml           # pnpm workspace definition
```

---

## 🧪 Testing & Verification

1. Open `artifacts/secret-agent-terminal/index.html` in your browser.
2. Open the Developer Tools console (`Cmd + Option + J` on macOS or `Ctrl + Shift + J` on Windows/Linux).
3. Reload the page to execute the built-in assertions.
4. Verify all tests pass cleanly without assertion failures.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

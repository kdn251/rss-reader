# Lab 1: Hands-on CLAUDE.md Creation

Build an RSS feed reader with Claude Code, then learn how to guide Claude's output by writing a CLAUDE.md file.

## Prerequisites

- Node.js installed
- A terminal and web browser
- Claude Code installed:
  ```bash
  npm install -g @anthropic-ai/claude-code
  ```

## Getting Started

1. Fork this repo on GitHub (click the "Fork" button at the top right)
2. Clone **your fork**:
   ```bash
   git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
   cd REPO-NAME
   ```
3. Start Claude Code:
   ```bash
   claude
   ```
4. Claude will ask for permissions as it works (read files, run commands, etc.). Type `y` to allow, or run `/permissions` to allow all for this session.
5. Give Claude this prompt:
   ```
   build me a website for reading rss feeds. use react with typescript for the frontend and typescript for the backend. create 2 directories one for the frontend and one for the backend.i want to be able to add feeds and browse the articles
   ```
6. Once generated, start both servers:
   ```bash
   cd server && npm install && npm run dev    # Terminal 1
   cd client && npm install && npm run dev    # Terminal 2
   ```
7. Open http://localhost:5173/ in your browser

## Test Feeds

See `feeds.txt` for a list of RSS feed URLs you can use to test your reader.

## What You'll Do

1. **Generate** the app with the vague prompt above
2. **Use** the app — add feeds, browse articles, try to break it
3. **Identify** what Claude got wrong (and why)
4. **Write** a CLAUDE.md file to capture rules and conventions
5. **Ask Claude** to update the codebase based on your CLAUDE.md
6. **See the difference** — same codebase, better output, just from adding context

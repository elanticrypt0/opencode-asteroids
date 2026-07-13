# Agent Notes — Asteroids

This is a minimal, dependency-free HTML5 Canvas game. There is no build system, package manager, test suite, or CI.

## Project structure

- `index.html` — entry point; loads `game.js` and creates an 800×600 canvas.
- `game.js` — all game logic, rendering, input, and state in one vanilla ES6+ file.
- `favicon.svg` — favicon only.

## How to run

Open `index.html` directly in a browser, or serve the repo root locally:

```bash
npx serve .
# then visit http://localhost:3000
```

There are no install, build, or watch steps.

## Conventions

- No frameworks, bundler, or external dependencies.
- Canvas dimensions are hardcoded to `800×600` in both `index.html` and `game.js` (constants `W`/`H`). Keep them in sync if you change the size.
- UI text and comments are in Spanish; README is in Spanish.
- `'use strict'` at the top of `game.js`.

## What to avoid

- Don't add a build pipeline unless explicitly asked — the project is intentionally zero-tooling.
- Don't split `game.js` into modules unless asked; the single-file style is intentional.

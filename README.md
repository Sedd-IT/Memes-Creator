# Meme Generator

A simple meme generator built with **React** and **Vite**. Pick an image, add your own text, and create a meme.

**Live demo:** `https://sedd-it.github.io/Memes-Creator/`

## Tech Stack

- [React 19](https://react.dev/)
- [Vite](https://vite.dev/) with [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react)
- [Oxlint](https://oxc.rs/docs/guide/usage/linter) for linting
- [gh-pages](https://github.com/tschaub/gh-pages) for deployment to GitHub Pages

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- npm

### Installation

```bash
git clone https://github.com/sedd-it/Memes-Creator.git
cd Memes-Creator
npm install
```

### Run locally

```bash
npm run dev
```

Then open the URL shown in your terminal (usually `http://localhost:5173/Memes-Creator/`).

## Available Scripts

| Command             | Description                                   |
| ------------------- | --------------------------------------------- |
| `npm run dev`       | Start the development server with HMR         |
| `npm run build`     | Create a production build in `dist/`          |
| `npm run preview`   | Preview the production build locally          |
| `npm run deploy`    | Build and publish `dist/` to GitHub Pages     |

## Project Structure

```
.
├── index.html          # App entry HTML
├── vite.config.js      # Vite config (base path set for GitHub Pages)
├── .oxlintrc.json      # Oxlint rules
├── package.json
└── src/
    ├── index.jsx       # React entry point
    ├── index.css       # Global styles
    └── photos/         # Images and assets (e.g. Troll.png favicon)
```

## Deployment

The project is set up for GitHub Pages:

1. Make sure `base` in `vite.config.js` matches your repository name:
   ```js
   base: '/Memes-Creator/',
   ```
2. Run:
   ```bash
   npm run deploy
   ```
   This builds the app and pushes the `dist` folder to the `gh-pages` branch.
3. In your repo, go to **Settings → Pages** and set the source to the `gh-pages` branch.

## Linting

```bash
npx oxlint
```

Rules are configured in `.oxlintrc.json` (React hooks rules and component export checks).

## License

This project is open source. Add a license of your choice (e.g. MIT) if you plan to share it.

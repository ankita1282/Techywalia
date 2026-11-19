# TECHYWALIA 6.0 — Mission Control

A React + Vite technical-festival concept website.

The Event Universe, quiz, project filters and Innovation Lab demo
work without an API key.

The assistant uses a local fallback until the optional server
function is deployed and configured.

## Run locally

1. Install Node.js (LTS).
2. Open this project folder.
3. Open a terminal inside the folder.
4. Run:

npm install

npm run dev

5. Open the local URL printed by Vite.
   Usually: http://localhost:5173

## Build

Run:

npm run build

npm run preview

## Optional real Gemini assistant on Vercel

1. Push this project to a GitHub repository.
2. Import the repository into Vercel.
3. In Vercel Project Settings > Environment Variables, add:

Name: GEMINI_API_KEY

Value: Your private Gemini API key

4. Redeploy the project.

The server function is in api/assistant.js.

Do not put the key in React code.
Do not use a VITE_ prefix.
Do not commit a real .env file.

## Important customization

- Replace sample project content in src/App.jsx with confirmed event information.
- Replace sample quiz questions with your own technical questions.
- The Innovation Lab currently uses local sample logic.
- The leaderboard and project showcase are demo content, not live event data.

## Deploy

Build command:

npm run build

Output directory:

dist

The optional /api/assistant endpoint is a Vercel serverless function.
If you deploy only the static dist folder to another host,
that function will not be included.
# CI-CD Demo

This demo contains a minimal Vue 3 frontend and an Express backend, plus a GitHub Actions workflow to:
- run tests (placeholder),
- build frontend,
- deploy frontend to Firebase Hosting (placeholder action),
- deploy backend to Heroku (placeholder action).

## How to run locally

### Backend
```
cd backend
npm install
node index.js
# server runs at http://localhost:3000
```

### Frontend
```
cd frontend
npm install
npm install @vitejs/plugin-vue --save-dev
npm run dev
# frontend runs (default) at http://localhost:5173
```

## Notes
- CI/CD workflow file uses GitHub Actions with example steps. You need to set GitHub Secrets (`FIREBASE_SERVICE_ACCOUNT`, `HEROKU_API_KEY`) and replace `your-firebase-project-id` and `your-heroku-app-name` with your real values before it will deploy.
- Tests are placeholders; add Jest/Vitest as you progress.
"//test $(date)" 

# Emoti Sense Guardian

This is my academic project for sentiment analysis in emergency calls.

The application provides:

- User and admin portals
- Emergency call transcript handling
- AI-assisted sentiment and urgency analysis
- Dataset and analytics views
- Contact and alert workflows

## Tech Stack

- React 18 + TypeScript
- Vite
- Tailwind CSS + shadcn/ui
- React Router
- TanStack Query
- Supabase (auth, database, edge functions)

## Project Context

This project explores NLP-driven emergency communication analysis using:

- JST (Joint Sentiment-Topic) modeling
- MEDLDA/SVM style classification workflow

## Local Setup

### 1) Prerequisites

- Node.js 18+ (recommended)
- npm

### 2) Install dependencies

```bash
npm install
```

### 3) Configure environment

Create a `.env` file in the project root and add:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_publishable_key

VITE_EMAILJS_SERVICE_ID=your_emailjs_service_id
VITE_EMAILJS_TEMPLATE_ID=your_emailjs_template_id
VITE_EMAILJS_PUBLIC_KEY=your_emailjs_public_key
```

### 4) Start development server

```bash
npm run dev
```

App runs on the local Vite URL shown in terminal (usually `http://localhost:5173`).

## Available Scripts

- `npm run dev` - start dev server
- `npm run dev:https` - start dev server (HTTPS mode in Vite config)
- `npm run build` - production build
- `npm run build:dev` - development-mode build
- `npm run lint` - run ESLint
- `npm run preview` - preview production build locally

## Main Routes

- `/` - Landing page
- `/auth` - Authentication page
- `/user-portal` - User dashboard
- `/admin-portal` - Admin dashboard

## Supabase

This repository includes Supabase resources:

- Edge functions under `supabase/functions/`
- SQL migrations under `supabase/migrations/`

If you are running the full backend stack, configure your Supabase project and deploy functions/migrations accordingly.

## Notes

- This README is project-specific and maintained manually.
- Replace environment placeholders with your actual keys before running all features.

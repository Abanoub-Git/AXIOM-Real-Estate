# AXIOM V2

AI-powered real estate platform for the Egyptian market.

**Stack:** Next.js 16 · FastAPI · Supabase · Ollama · TypeScript · Python 3.11

---
## Screenshots

### 1. Home Page
![Home Page](./website%20screenshots/1.png)

### 2. Find Homes
![Find Homes](./website%20screenshots/2.png)

### 3. Agencies
![Agencies](./website%20screenshots/3.png)

### 4. Universities
![Universities](./website%20screenshots/4.png)

### 5. Pricing
![Pricing](./website%20screenshots/5.png)

### 6. Blog
![Blog](./website%20screenshots/6.png)

### 7. User Dashboard
![User Dashboard](./website%20screenshots/7.png)

### 8. AI Assistant
![AI Assistant](./website%20screenshots/8.png)

### 9. Admin Dashboard
![Admin Dashboard](./website%20screenshots/9.png)

### 10. Authentication
![Authentication](./website%20screenshots/10.png)

### 11. Login
![Login](./website%20screenshots/11.png)

### 12. Sign Up
![Sign Up](./website%20screenshots/12.png)

## Quick Start

### Frontend
```bash
cd frontend
npm install
npm run dev        # http://localhost:3000
```


### Backend
```bash
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000   # http://localhost:8000
```

### AI (Ollama)
```bash
ollama pull nomic-embed-text
ollama create axiom-llm -f path/to/Modelfile
```

---

## Features

- Property listings — for sale, for rent, shared housing
- AI chatbot with RAG and inline listing cards (SSE streaming)
- Natural language property search (filter extraction + pgvector)
- Personalized recommendations and shared-housing compatibility scoring
- Listing description generator (bilingual AR/EN)
- AI amenity content moderation
- Fraud detection scoring
- Dashboard with listing management, saved homes, and profile settings
- Admin approval queue for listings

---

## Pages

| Route | Description |
|-------|-------------|
| `/` | Homepage |
| `/find-homes` | Property search with filters and NLP |
| `/property/[id]` | Property detail (all categories incl. shared housing) |
| `/dashboard` | User dashboard: listings, saved homes, profile |
| `/messages` | Removed: WhatsApp lead capture replaces in-app messaging |
| `/agencies` | Real estate developers directory |
| `/agencies/[slug]` | Agency detail with projects and listings |
| `/project/[id]` | Development project detail |
| `/blog` | Blog listing |
| `/admin/dashboard` | Admin panel |

---

## Docs

- `FULLknowledge.md` — **Complete learning guide** — novice to expert on every layer (start here)
- `docs/API_REFERENCE.md` — Backend endpoint contracts
- `docs/BACKEND.md` — Backend architecture reference
- `docs/AI_FEATURES.md` — AI feature specs
- `docs/SETUP.md` — Detailed setup guide
- `docs/ROADMAP.md` — Current status and next steps

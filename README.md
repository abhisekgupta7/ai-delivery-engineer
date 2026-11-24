# AI Delivery Engineer

A full-stack application for AI-assisted software delivery operations.

## Structure

- `frontend/` - Next.js application
- `backend/` - FastAPI application
- `docker-compose.yml` - Local frontend and backend services
- `.github/workflows/` - CI workflows

## Run locally

Start the backend:

```powershell
cd backend
python -m pip install -r requirements.txt
python -m uvicorn app.main:app --reload --port 8000
```

Start the frontend:

```powershell
cd frontend
npm install
npm run dev
```

Open http://localhost:3000. The backend health endpoint is available at http://localhost:8000/health.

## Docker Compose

```powershell
docker compose up --build
```

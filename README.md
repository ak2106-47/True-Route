# True Route

Flight delays and cancellations cause stress, missed connections, and wasted time. As a result, I tried to reinforce the need for a smarter way to choose reliable flights. I wanted to build a solution that helps travelers avoid disruptions by using data-driven predictions, ensuring a smoother travel experience..

## Setup

### 1. Backend (Flask + MongoDB)

```bash
cd backend
python -m venv venv
source venv/bin/activate          # On Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env
# Then edit .env and fill in your MongoDB connection string
python app.py
```

### 2. Frontend (React + Vite)

```bash
cd frontend
npm install
cp .env.example .env
# Then edit .env and fill in your API keys
npm run dev
```

## Required API Keys

The frontend uses several third-party APIs. You'll need to register and get keys for:

- **Aviation API** ([aviationstack.com](https://aviationstack.com/)) — for live flight data
- **SerpAPI** ([serpapi.com](https://serpapi.com/)) — for search results

The backend needs:

- **MongoDB Atlas** ([cloud.mongodb.com](https://cloud.mongodb.com/)) — free tier is fine

## Project Structure

```
TrueRoute/
├── backend/        # Flask API, scoring logic, MongoDB integration
└── frontend/       # React + Vite UI
```

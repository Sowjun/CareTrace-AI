# CareTrace AI

CareTrace AI is a health monitoring platform built using FastAPI and React.
The project focuses on tracking health metrics, managing medical reports, and providing AI-assisted health insights through a simple and responsive interface.

## Features

* Health metrics tracking
* AI-based health analysis
* Medical report upload and management
* Timeline-based health history
* Smart health alerts
* Multi-language support
* JWT authentication
* Responsive UI with dark/light mode

---

## Tech Stack

### Backend

* FastAPI
* MongoDB
* Motor
* JWT Authentication
* Pytest

### Frontend

* React
* Vite
* TailwindCSS
* React Router
* i18next
* Recharts

---

## Project Structure

```bash
care-trace-ai-demo/
├── backend/
├── frontend/
├── README.md
├── package.json
└── render.yaml
```

---

## Getting Started

### Prerequisites

* Python 3.9+
* Node.js 18+
* MongoDB Atlas or local MongoDB

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Sowjun/CareTrace-AI.git
cd care-trace-ai-demo
```

### 2. Install dependencies

```bash
npm run install:frontend
npm run install:backend
```

### 3. Configure environment variables

Create a `.env` file in the root directory.

```env
MONGO_URI=your_mongodb_uri
DB_NAME=caretrace_ai
SECRET_KEY=your_secret_key
ACCESS_TOKEN_EXPIRE_MINUTES=10080
CORS_ORIGINS=http://localhost:5173
```

Generate a secret key:

```bash
python -c "import secrets; print(secrets.token_hex(32))"
```

---

## Run the Project

```bash
npm run dev
```

### Application URLs

Frontend:

```bash
http://localhost:5173
```

Backend:

```bash
http://127.0.0.1:8001
```

API Docs:

```bash
http://127.0.0.1:8001/docs
```

---

## Available Commands

```bash
npm run dev
npm run dev:backend
npm run dev:frontend
npm run build
npm run test
```

---

## Deployment

### Backend

Deploy using Render or any FastAPI-supported hosting service.

### Frontend

Deploy using Vercel.

Make sure to update:

* `CORS_ORIGINS`
* `VITE_API_URL`

before production deployment.

---

## Demo Account

```text
Email: rahul@demo.com
Password: demo1234
```

---

## Security

The project includes:

* JWT authentication
* Password hashing
* Input validation
* File upload validation
* Secure environment variable handling

---

## Testing

### Backend

```bash
cd backend
pytest tests/ -v
```

### Frontend

```bash
cd frontend
npm test
```

---

## License

This project is licensed under the MIT License.

---

## Disclaimer

This project is built for educational and research purposes and is not intended for real-world clinical use without proper medical validation.

# CareerAI — AI-Powered Recruitment Platform

<div align="center">

**Empowering smarter hiring through AI-driven recruitment solutions.**

CareerAI is a full-stack AI-powered recruitment platform that analyzes job descriptions, processes candidate profiles, performs semantic matching using vector embeddings, ranks candidates based on relevance, and generates context-aware interview questions.

</div>

---

## 🚀 Features

### 🤖 AI-Powered Recruitment

* **AI Job Analysis** — Analyze job descriptions and identify important skills and requirements.
* **Smart Candidate Matching** — Match candidates with job descriptions using semantic similarity and vector embeddings.
* **Candidate Ranking** — Rank candidates based on their relevance to a job.
* **Interview Question Generation** — Generate context-aware interview questions based on job requirements and candidate profiles.

### 👤 Candidate Management

* Upload and manage candidate profiles.
* Add individual candidates.
* Process candidate information for matching.
* View candidate matching results.

### 🔐 Authentication

* Auth0-based authentication.
* Protected application routes.
* Backend authentication and authorization.
* Secure environment-based configuration.

### ⚡ Full-Stack Architecture

* React + TypeScript frontend.
* Flask/Python backend.
* RESTful API architecture.
* Pinecone vector database.
* OpenAI embeddings.
* Responsive Tailwind CSS interface.
* Docker-based development support.

---

## 🧠 How CareerAI Works

```text
                    CareerAI
                       │
          ┌────────────┴────────────┐
          ↓                         ↓
   Job Description              Candidate
          │                       Profile
          ↓                         ↓
     Job Analysis             Candidate Processing
          │                         │
          └────────────┬────────────┘
                       ↓
                Text Embeddings
                       ↓
               Pinecone Vector DB
                       ↓
              Semantic Similarity
                       ↓
              Candidate Ranking
                       ↓
          ┌────────────┴────────────┐
          ↓                         ↓
     Match Results          Interview Questions
```

### Semantic Matching

CareerAI uses vector embeddings to compare the meaning of candidate profiles with job requirements rather than relying only on exact keyword matches.

```text
Job Description
       ↓
   Embedding
       ↓
Vector Representation
       ↓
Semantic Similarity
       ↑
Vector Representation
       ↑
   Embedding
       ↑
Candidate Profile
```

---

## 🛠️ Tech Stack

### Frontend

* React 18
* TypeScript
* Vite
* React Router
* Tailwind CSS
* Framer Motion
* Auth0 React SDK

### Backend

* Python
* Flask
* REST APIs
* Authentication & Authorization

### AI & Vector Search

* OpenAI Embeddings
* Pinecone
* Semantic Similarity Search

### Infrastructure

* Docker
* Docker Compose
* Nginx
* Vercel

---

## 📁 Project Structure

```text
CareerAI/
│
├── src/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   ├── lib/
│   ├── types/
│   └── main.tsx
│
├── backend/
│   ├── config/
│   ├── database/
│   ├── models/
│   ├── routes/
│   ├── src/
│   ├── tests/
│   └── utils/
│
├── config/
│   ├── environments/
│   └── production/
│
├── docs/
├── Dockerfile
├── docker-compose.yml
├── nginx.conf
├── package.json
├── vite.config.ts
└── README.md
```

---

## 📦 Installation

### Prerequisites

* Node.js 16+
* npm
* Python 3.8+
* OpenAI API key
* Pinecone account and API key
* Auth0 configuration

### Clone the repository

```bash
git clone https://github.com/mokallasathvik23/CareerAI.git

cd CareerAI
```

### Install frontend dependencies

```bash
npm install
```

### Install backend dependencies

```bash
pip install -r requirements.txt
```

### Configure environment variables

Create a `.env` file based on `.env.example`.

```env
OPENAI_API_KEY=your_openai_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_ENVIRONMENT=your_pinecone_environment
DEBUG=True
```

> Never commit API keys, passwords, JWT secrets, or other sensitive credentials to GitHub.

---

## ▶️ Running the Application

### Start the backend

```bash
python app.py
```

The backend runs on:

```text
http://localhost:5000
```

### Start the frontend

```bash
npm run dev
```

The frontend runs on:

```text
http://localhost:5173
```

---

## 🎯 Usage

### 1. Analyze a Job Description

Enter a job description into CareerAI.

The system analyzes the job requirements and identifies relevant skills.

### 2. Add Candidates

Upload candidate profiles or add candidates through the application.

### 3. Match Candidates

CareerAI processes candidate and job information using embeddings and semantic similarity.

### 4. View Candidate Rankings

Candidates are ranked according to their similarity to the selected job.

### 5. Generate Interview Questions

Generate interview questions based on the job requirements and candidate information.

---

## 🔌 API Endpoints

### Jobs

```text
POST /jobs/analyze
```

Analyze a job description.

```text
GET /jobs/
```

Get job endpoint information.

### Candidates

```text
POST /candidates/upload
```

Upload multiple candidates.

```text
POST /candidates/add
```

Add an individual candidate.

### Interview Questions

```text
POST /questions/generate
```

Generate AI-powered interview questions.

```text
POST /questions/submit
```

Submit and evaluate interview answers.

---

## 🐳 Docker

Build the application:

```bash
docker-compose build
```

Start the services:

```bash
docker-compose up
```

Stop the services:

```bash
docker-compose down
```

---

## 🧪 Development Commands

```bash
# Start development server
npm run dev

# Build production application
npm run build

# Preview production build
npm run preview

# Type checking
npm run type-check

# Start Docker services
docker-compose up

# Stop Docker services
docker-compose down
```

---

## 🔐 Security

CareerAI uses environment variables for sensitive configuration.

The following should never be committed to GitHub:

```text
.env
API keys
OpenAI credentials
Pinecone credentials
JWT secrets
Auth0 secrets
```

Use `.env.example` to document required configuration without exposing real credentials.

---

## 📸 Screenshots

Add screenshots of your **CareerAI application** here.

Recommended screenshots:

* Landing page
* Login/authentication
* CareerAI dashboard
* Job analysis
* Candidate upload
* Candidate ranking
* Matching results
* Interview question generation

Example:

```markdown
![CareerAI Dashboard](screenshots/dashboard.png)

![Job Analysis](screenshots/job-analysis.png)

![Candidate Matching](screenshots/candidate-matching.png)
```

---

## 🔮 Future Improvements

* Resume PDF parsing
* Automatic skill extraction from resumes
* Skill-gap analysis
* Personalized job recommendations
* Candidate application tracking
* Recruiter analytics dashboard
* Advanced candidate filtering
* Interview preparation workspace
* Improved candidate ranking algorithms
* Automated testing
* Production cloud deployment

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch.

```bash
git checkout -b feature/your-feature
```

3. Commit your changes.

```bash
git commit -m "Add your feature"
```

4. Push the branch.

```bash
git push origin feature/your-feature
```

5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## 🙏 Acknowledgments

* OpenAI for embedding and AI capabilities.
* Pinecone for vector search infrastructure.
* React community.
* Flask community.
* Tailwind CSS community.

---

<div align="center">

**Built with AI to connect the right talent with the right opportunities.**

### CareerAI

</div>

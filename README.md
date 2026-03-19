# AI Radar Resume Parser

An advanced AI-powered resume parser and candidate matching system.

## Features

- **Resume Parsing**: Extracts text and key information from uploaded resumes.
- **AI Analysis**: Uses Groq (LLM) to analyze resumes against job descriptions.
- **Job Management**: Create and manage job postings.
- **Candidate Analysis**: View detailed analysis and scoring of candidates with interactive Radar Charts.
- **Premium Authentication**: A futuristic, glassmorphism-styled login and signup experience with secure JWT-based session management.
- **Chat Interface**: Context-aware chat to query candidate data.
- **Modern UI**: Built with Next.js and Tailwind CSS with a cinematic, data-center aesthetic.

## Tech Stack

- **Frontend**: Next.js, React, Tailwind CSS, TypeScript, Framer Motion
- **Backend**: FastAPI, Python, SQLAlchemy, SQLite (via PBKDF2 hashing)
- **AI/LLM**: Groq Cloud API
- **Containerization**: Docker, Docker Compose

## Prerequisites

- [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/) installed.
- [Groq API Key](https://console.groq.com/keys) (for AI functionality).

## Setup & Running

1. **Clone the repository**:
   ```bash
   git clone https://github.com/AllyanSystumm/AI-Radar-Resume.git
   cd AI-Radar-Resume
   ```

2. **Configure Environment Variables**:
   
   Navigate to the `backend` directory and ensure you have a `.env` file with your API keys:
   ```bash
   # backend/.env
   GROQ_API_KEY=your_groq_api_key_here
   HF_TOKEN=your_huggingface_token_here
   ```

3. **Run with Docker Compose**:

   From the project root directory, run:
   ```bash
   docker-compose up --build
   ```

4. **Access the Application**:
   - **Frontend**: [http://localhost:3000](http://localhost:3000)
   - **Backend API Docs**: [http://localhost:8001/docs](http://localhost:8001/docs)

## Project Structure

- `backend/`: FastAPI application, database models, and services.
- `frontend/`: Next.js frontend application.
- `docker-compose.yml`: Docker services configuration.

## Usage

1. **Sign In**: Access the futuristic login page and create an account or sign in.
2. **Create a Job**: After sign-in, you are automatically taken to the job creation dashboard.
3. **Apply**: Use the application form to upload a resume for a specific job.
4. **View Analysis**: Check the job dashboard to see ranked candidates and detailed AI analysis with Radar Charts.
5. **Chat**: Use the chat interface to ask questions about the candidates.
   - **Integrated Chatbot**: The recruiter can ask directly, for example: "Give me the top scorer of the graphic designing job". The chatbot has full access to the database and can query candidate information.

<img width="1647" height="892" alt="Application Overview" src="https://github.com/user-attachments/assets/c8dab815-beab-42a4-b14e-96d06b5361c8" />
<img width="1647" height="892" alt="Futuristic Login UI" src="frontend/public/login-bg.png" />

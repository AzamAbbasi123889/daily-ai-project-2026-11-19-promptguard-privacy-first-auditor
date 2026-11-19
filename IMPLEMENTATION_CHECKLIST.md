# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] Returns a numeric risk score 0‑100
- [ ] Risk > 70 triggers injection_flag=True
- [ ] False‑positive rate measured on the provided benchmark < 10%
- [ ] Leakage score > 0.5 flags leakage_flag=True
- [ ] No raw PII is persisted beyond 24 h
- [ ] Detection precision ≥ 85% on synthetic test set
- [ ] Response latency ≤ 500 ms for cold cache
- [ ] Proper HTTP 401 on missing/invalid API key
- [ ] Audit record written to PostgreSQL
- [ ] Shows last 50 audits
- [ ] Aggregates average risk and leakage over time
- [ ] Set up FastAPI skeleton with API‑key middleware
- [ ] Implement PostgreSQL schema + pgvector extension
- [ ] Containerize services with Docker‑Compose
- [ ] Integrate contrastive prototype detector (load pretrained weights)
- [ ] Build leakage scorer using spaCy + regex
- [ ] Unit tests for injection detector wrapper (pytest)
- [ ] Unit tests for leakage scorer functions
- [ ] Integration tests for /audit endpoint (requests)
- [ ] Security tests: verify API‑key enforcement and SQL injection resistance
- [ ] Load test with Locust to validate latency SLA
- [ ] Build multi‑stage Docker images (builder + runtime)
- [ ] Push to GitHub Container Registry via GitHub Actions on each merge
- [ ] Deploy to Railway (free tier) using docker‑compose.yml
- [ ] Configure automated health checks and rolling restarts

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.

# CivivLens - – AI-Powered Transparency & Accountability Platform
CivicLens uses generative AI and public data APIs to make government transparency, community impact, and public project spending more accessible to citizens. It automatically aggregates open government datasets, budget reports, and procurement documents — then uses Geminito translate them into plain language insights, dashboards, and alerts.

https://gemini.google.com/share/d791ee639246

<img width="1536" height="1024" alt="IMG_1316" src="https://github.com/user-attachments/assets/9f0c9fa6-65c5-4ab7-9fe4-ed89ed477964" />


https://vimeo.com/1130778641

CivicLens is an AI-powered transparency assistant that transforms complex government data into easy-to-understand insights. It empowers citizens, journalists, and policymakers with clear, fact-based summaries and visual analytics about how public funds are allocated and spent.

🌍 Goal
Use AI Studio + Gemini + Cloud Run to:
* Automatically summarize open government datasets.
* Provide a conversational AI (“Ask CivicLens”) for data exploration.
* Detect irregular spending using anomaly detection models.
* Deploy the entire application serverlessly with Cloud Run.

🧩 Core Features
Module	Description
🧠 AI Summarizer	Ingests public datasets (CSV, JSON, PDF) → Summarizes them using Gemini in plain language.
💬 Civic Q&A Bot	Natural-language chatbot powered by Gemini — answers questions like “Where did my tax money go?”.
💰 Spending Visualizer	Next.js frontend with charts and maps (by region, sector, or project).
⚠️ Anomaly Detector	ML model (BigQuery ML + Gemini reasoning) flags unusual spending patterns.
🔐 Secure Gateway	OAuth2 with Google Identity; stores only anonymized and public data.
☁️ Serverless Infra	Fully deployed on Cloud Run with CI/CD, Pub/Sub, and Firestore integration
Tech Stack: Gemini + AI Studio + Cloud Run + BigQuery + Firestore + Pub/Sub

🧩 Key Features
1. AI Transparency Summaries — Converts dense reports (PDFs, CSVs, or APIs) into human-readable summaries.
2. Budget Breakdown Generator — Visualizes how funds are allocated across public projects.
3. Civic Chatbot (Ask CivicLens) — Gemini chatbot that answers questions like “How much was spent on education in 2024?” or “Which contractors won road repair bids?”
4. Anomaly Detection — Uses Gemini + BigQuery ML to detect irregularities in spending patterns.
5. Citizen Portal — Web interface deployed on Cloud Run with feedback submission and open data links.

🏗️ Architecture Overview
* Frontend: Next.js + TailwindCSS on Cloud Run (Service A)
* Backend API: Flask + FastAPI microservice for Gemini integration (Service B)
* Data Layer: BigQuery + Firestore (for caching summaries)
* AI Core: Gemini 1.5 Flash + Vertex AI + Pub/Sub for async processing
* CI/CD: GitHub Actions auto-deploy to Cloud Run
* Security: OAuth2 (Google Identity), role-based data access

🧠 Impact
Empowers citizens, journalists, and NGOs to understand governance decisions without needing data science expertise. Increases transparency, encourages civic engagement, and fosters trust between the public and institutions.

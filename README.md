# CivivLens - – AI-Powered Transparency & Accountability Platform
CivicLens uses generative AI and public data APIs to make government transparency, community impact, and public project spending more accessible to citizens. It automatically aggregates open government datasets, budget reports, and procurement documents — then uses Geminito translate them into plain language insights, dashboards, and alerts.

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

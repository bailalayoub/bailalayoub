<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/banner-light.svg">
  <img src="https://github.com/bailalayoub/bailalayoub/raw/main/assets/banner-light.svg" width="100%" alt="Ayoub Bailal, Software Engineer · Backend Go · Microservices · Applied AI (RAG, LLM agents) · Cloud">
</picture>

**Scalable architecture | Generative AI | DevOps | Fullstack React/TypeScript**

<a href="https://www.linkedin.com/in/ayoubbailal"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://medium.com/@bailalayoub"><img src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white" alt="Medium"></a>
<a href="https://www.bailalayoub.com/"><img src="https://img.shields.io/badge/Portfolio-2563EB?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"></a>

<sub>
<a href="#about-me">About</a> ·
<a href="#featured-rebound">Rebound</a> ·
<a href="#projects">Projects</a> ·
<a href="#skills--tech-stack">Skills</a> ·
<a href="#experience">Experience</a> ·
<a href="#github-stats">Stats</a> ·
<a href="#education">Education</a> ·
<a href="#extracurricular--events">Events</a> ·
<a href="#contact-me">Contact</a>
</sub>

</div>

---

## About Me

<img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" align="right" width="180" alt="Animated illustration of a developer coding at a desk">

IT engineer from **ENSAO**, with **2+ years of experience** as a Software Engineer on an EdTech platform. I specialise in **Go** backend development in a **microservices** architecture (secure APIs, PostgreSQL, Redis, MinIO), in **generative AI** features (RAG, embeddings, LLM agents, OpenAI integration), and in cloud deployment with **Docker** and **CI/CD**.

I care about systems that stay correct when the network, the model or the server does not. I work across the stack, from infrastructure and databases to **React/TypeScript** interfaces.

<br clear="right">

---

## Featured: Rebound

<a href="https://github.com/bailalayoub/rebound">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/rebound-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/rebound-light.svg">
    <img src="https://github.com/bailalayoub/bailalayoub/raw/main/assets/rebound-light.svg" width="100%" alt="Rebound: a generation goroutine writes to a numbered log in memory or Redis Streams; an SSE client resumes from its Last-Event-ID. About 104,000 reconnections across 12 scenarios, zero failures. Go, Redis Streams, Lua, TypeScript.">
  </picture>
</a>

**[Rebound](https://github.com/bailalayoub/rebound)** is an open-source Go library that makes streamed LLM answers resumable. When a connection drops, the client picks up exactly where it left off, on any server: no gap, no duplicate, no answer generated twice.

- The generation runs in its own goroutine, detached from the HTTP request, and writes to a numbered log (in memory, or Redis Streams with atomic Lua scripts).
- Every SSE client reads that log from its `Last-Event-ID`. Replay and live are the same read.
- `net/http` and Gin adapters, a dependency-free TypeScript client, and a conformance tester that drops connections at random: about 104,000 reconnections across 12 scenarios, zero failures.

📖 Read the story: [Your LLM answer shouldn't die with the HTTP connection](https://medium.com/@bailalayoub/your-llm-answer-shouldnt-die-with-the-http-connection-d97be23a6a74)

---

## Projects

<table>
<tr>
<td width="50%" valign="top">
<b><a href="https://github.com/bailalayoub/rebound">Rebound</a></b><br>
Open-source library for resumable LLM streams over SSE, multi-instance with Redis<br><br>
<code>Go</code> <code>Redis&nbsp;Streams</code> <code>Lua</code> <code>TypeScript</code>
</td>
<td width="50%" valign="top">
<b>Supplier offer ingestion platform</b> <sub>(freelance)</sub><br>
Turns unstructured supplier offers (email, WhatsApp, PDF, Excel, images) into validated product data: event-driven pipeline, LLM extraction with deterministic business rules, dead-letter queue, token budget, human review<br><br>
<code>Python</code> <code>FastAPI</code> <code>PostgreSQL</code> <code>Redis</code> <code>Claude&nbsp;API</code> <code>AWS&nbsp;S3</code> <code>React</code>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<b>Tilmid+</b><br>
Adaptive AI tutor: RAG treated as a data pipeline (OCR, chunking, embeddings, Qdrant), LangGraph agents with tool calling, real-time SSE chat, 3D learning world<br><br>
<code>Go</code> <code>Python</code> <code>LangGraph</code> <code>OpenAI</code> <code>Qdrant</code> <code>React</code> <code>Three.js</code>
</td>
<td width="50%" valign="top">
<b>Tilmicode</b><br>
E-learning platform that teaches programming to children: Blockly, Phaser mini-games, Python editor, FR/EN/AR with Arabic RTL, online payment<br><br>
<code>Go</code> <code>Gin</code> <code>Python</code> <code>PostgreSQL</code> <code>MinIO</code> <code>React</code>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<b>TilmiSchool</b><br>
Multi-tenant school management SaaS with per-tenant isolation and SSO shared across three applications<br><br>
<code>Go</code> <code>Gin</code> <code>PostgreSQL</code> <code>React</code> <code>Docker</code>
</td>
<td width="50%" valign="top">
<b>Cloud data platform</b><br>
Three-layer data platform on Google Cloud with encryption before storage<br><br>
<code>Pub/Sub</code> <code>Dataflow</code> <code>BigQuery</code> <code>Cloud&nbsp;Run</code>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<b>GENANO, anonymisation engine</b><br>
Configuration-driven encryption, hashing and anonymisation of JSON, CSV, XML, TXT, HTML, DOCX and XLSX, plus synthetic data generation<br><br>
<code>Python</code> <code>FastAPI</code> <code>Cloud&nbsp;Run</code> <code>Cloud&nbsp;Storage</code>
</td>
<td width="50%" valign="top">
<b><a href="https://www.bailalayoub.com/">3D portfolio</a></b><br>
Personal portfolio as a navigable 3D experience<br><br>
<code>Next.js</code> <code>TypeScript</code> <code>React&nbsp;Three&nbsp;Fiber</code> <code>GSAP</code>
</td>
</tr>
</table>

<details>
<summary><b>Academic projects</b> (4)</summary>
<br>

<table>
<tr>
<td width="50%" valign="top">
<b>Vehicle detection</b> <sub>(academic)</sub><br>
Real-time vehicle detection and classification for urban traffic analysis<br><br>
<code>Computer&nbsp;vision</code> <code>Python</code>
</td>
<td width="50%" valign="top">
<b>Emotion detection</b> <sub>(academic)</sub><br>
Real-time emotion recognition from a webcam with a CNN trained on FER-2013<br><br>
<code>Python</code> <code>CNN</code>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<b>Traffic sign recognition</b> <sub>(academic)</sub><br>
Real-time traffic sign detection and classification<br><br>
<code>Computer&nbsp;vision</code> <code>Python</code>
</td>
<td width="50%" valign="top">
<b>Sales dashboard</b> <sub>(academic)</sub><br>
Executive sales report with fbprophet forecasting<br><br>
<code>Power BI</code> <code>Python</code>
</td>
</tr>
</table>

</details>

---

## Skills & Tech Stack

<table>
<tr>
<td><b>Languages</b></td>
<td>
<img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" alt="SQL">
</td>
</tr>
<tr>
<td><b>Frameworks & Libraries</b></td>
<td>
<img src="https://img.shields.io/badge/Gin-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Gin">
<img src="https://img.shields.io/badge/Gorilla_Mux-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Gorilla Mux">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain">
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangGraph">
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React">
<img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT">
</td>
</tr>
<tr>
<td><b>AI & Generative</b></td>
<td>
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI">
<img src="https://img.shields.io/badge/RAG_Pipeline-FF6B35?style=flat-square" alt="RAG Pipeline">
<img src="https://img.shields.io/badge/Embeddings-8A2BE2?style=flat-square" alt="Embeddings">
<img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square" alt="Qdrant">
<img src="https://img.shields.io/badge/SSE_Streaming-1a1a1a?style=flat-square" alt="SSE Streaming">
</td>
</tr>
<tr>
<td><b>Databases & Storage</b></td>
<td>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
<img src="https://img.shields.io/badge/MinIO-C72E49?style=flat-square&logo=minio&logoColor=white" alt="MinIO">
</td>
</tr>
<tr>
<td><b>Cloud & DevOps</b></td>
<td>
<img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="GCP">
<img src="https://img.shields.io/badge/Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Cloud Run">
<img src="https://img.shields.io/badge/BigQuery-4285F4?style=flat-square&logo=googlebigquery&logoColor=white" alt="BigQuery">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker Compose">
<img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white" alt="Nginx">
<img src="https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="CI/CD">
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus">
</td>
</tr>
<tr>
<td><b>Architecture & Patterns</b></td>
<td>
<img src="https://img.shields.io/badge/Microservices-FF6B35?style=flat-square" alt="Microservices">
<img src="https://img.shields.io/badge/API_Gateway-FF9900?style=flat-square" alt="API Gateway">
<img src="https://img.shields.io/badge/REST_API-02569B?style=flat-square" alt="REST">
<img src="https://img.shields.io/badge/Event_Driven-7C3AED?style=flat-square" alt="Event Driven">
<img src="https://img.shields.io/badge/Zap_Logger-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Zap Logger">
</td>
</tr>
<tr>
<td><b>Data Visualization</b></td>
<td>
<img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" alt="Power BI">
<img src="https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white" alt="Tableau">
</td>
</tr>
</table>

---

## Experience

### 🚀 Software Engineer · Tilmicode, Sidra platform
<sub>September 2024 → present</sub>

- Design of a **complete microservices ecosystem** (Go/Python) for education and AI
- Production **AI/RAG pipeline**: OCR, chunking, OpenAI embeddings, Qdrant vector search
- **Real-time AI chat** with SSE streaming, quota management and payment integration
- Subscription system with **scheduled activation** and inter-service orchestration
- Advanced **React/TypeScript** frontends: Blockly, Phaser and CodeMirror editors
- Large-scale storage (PostgreSQL, MinIO, Qdrant), migrations, asynchronous pipelines
- Full industrialisation: Docker, CI/CD, **Prometheus**, structured logging with Zap
- Inter-service security: JWT, internal tokens, CORS

### 💼 Freelance · Supplier offer ingestion platform
<sub>Client in the Netherlands</sub>

- Event-driven pipeline: webhook, queue, workers, LLM extraction, deterministic business rules, human review, export
- Idempotency, administrable dead-letter queue, controlled retries, fail-closed daily token budget

### 🎓 Final-year internship · Vision Business Consulting
<sub>February → July 2024</sub>

- Built **GENANO**: anonymisation, encryption and hashing across formats (JSON, CSV, TXT, XML)
- Deployment on **Google Cloud Platform** (Cloud Run, Dataflow, BigQuery, Cloud Functions)
- Pipelines for large structured, semi-structured and unstructured data transfers
- GitHub repositories, DevOps practices, monitoring of scheduled modules

---

## GitHub Stats

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/stats-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/stats-light.svg">
  <img src="https://github.com/bailalayoub/bailalayoub/raw/main/assets/stats-light.svg" alt="Ayoub Bailal's GitHub stats: stars, commits, pull requests, issues and contributions">
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/top-langs-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/bailalayoub/bailalayoub/raw/main/assets/top-langs-light.svg">
  <img src="https://github.com/bailalayoub/bailalayoub/raw/main/assets/top-langs-light.svg" alt="Most used languages across Ayoub Bailal's repositories">
</picture>

</div>

---

## Education

🎓 **École Nationale des Sciences Appliquées d'Oujda (ENSAO)**<br>
*Engineering degree in Information Technology and Communication Networks* · `2019 → 2024`

---

## Extracurricular & Events

| | Event | Role |
|---|---|---|
| 🎙️ | **GITEX Africa 2026** | Exhibitor with Tilmicode · Investor and startup meetings |
| 🤖 | **Assises Nationales de l'IA 2025** | Exhibitor with Tilmicode · UM6P · Ministry of Digital Transition |
| 🌍 | **GITEX Africa 2024** | Participant with Vision Business Consulting |
| 📰 | **MAGENSAO** <sub>2021 – 2023</sub> | Digital Team Leader · First ENSAO magazine |
| 🏛️ | **ITIRC Club** <sub>2021 – 2023</sub> | President · IT & Networks club, ENSAO |
| 🎨 | **EUGO** <sub>2022</sub> | Graphic Designer · National event, 500+ students |
| 🖼️ | **JPO Open Day** <sub>2023</sub> | Designer · 11th edition, ENSAO |

---

## Contact Me

<table>
<tr><td><b>Email</b></td><td><a href="mailto:bailalayoub4905@gmail.com">bailalayoub4905@gmail.com</a></td></tr>
<tr><td><b>Portfolio</b></td><td><a href="https://www.bailalayoub.com/">https://www.bailalayoub.com/</a></td></tr>
<tr><td><b>LinkedIn</b></td><td><a href="https://www.linkedin.com/in/ayoubbailal">https://www.linkedin.com/in/ayoubbailal</a></td></tr>
<tr><td><b>Medium</b></td><td><a href="https://medium.com/@bailalayoub">https://medium.com/@bailalayoub</a></td></tr>
<tr><td><b>Phone</b></td><td>+212 708342354</td></tr>
<tr><td><b>Location</b></td><td>Rabat, Morocco</td></tr>
</table>

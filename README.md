# Muhammad Faiq Imran

Software Engineering student (University of Stirling, RAK, UAE), building full-stack systems end to end — from database schema and REST APIs to the front end — and researching the machine-learning side of that stack: CNN ablation studies, cost-sensitive modeling, and neuroevolution for autonomous driving.

<!-- Verified links only: GitHub profile, portfolio, LinkedIn. -->
[![Portfolio](https://img.shields.io/badge/Portfolio-faiqimranportfolio.netlify.app-0C1421?style=flat-square&logo=googlechrome&logoColor=white)](https://faiqimranportfolio.netlify.app/)
[![GitHub](https://img.shields.io/badge/GitHub-ARTI--INTEL-10223F?style=flat-square&logo=github&logoColor=white)](https://github.com/ARTI-INTEL)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Muhammad%20Faiq%20Imran-162337?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-faiq-imran-99665a308/)

---

## Current focus

- **Full-stack engineering** — multi-tenant systems, JWT/RBAC auth, MySQL schema design, real-time features (WebSocket, WebRTC)
- **Machine learning research** — CNN architecture ablations on MNIST/EMNIST and cost-sensitive credit scoring (`Handwritten-Character-Recognition`, `Credit-Scoring-Model`, both recent)
- **Autonomous systems** — reinforcement learning with NEAT neuroevolution (`AI-Learns-to-Drive`)
- **ML internship work** — supervised learning fundamentals: honest validation, class imbalance, feature leakage, and metrics that match the business question

---

## Featured projects

All repositories are public; descriptions reflect what is actually implemented in each.

### 1. [Viron CAD](https://github.com/ARTI-INTEL/Viron-CAD)
A full Computer-Aided Dispatch platform for emergency-response roleplay communities — dispatch, departments, records, and real-time comms in one system.

- **Real-time voice radio** built on WebRTC with JWT-authenticated WebSocket signalling; per-department peer-to-peer mesh channels (LEO, Fire & Rescue, DOT, Dispatch)
- **Live ERLC game integration** — WebSocket player tracking, 911-call sync with deduplication, and server keys encrypted at rest (AES-256-GCM)
- **Discord + Roblox OAuth 2**, five distinct CAD views under role-based access, searchable character/vehicle/firearm records, and a server-scoped audit log

`Node.js · Express 5 · MySQL · WebRTC · ws · JWT · Electron · pdf-lib`

### 2. [Garage Management System](https://github.com/ARTI-INTEL/Garage-Management-Software)
Multi-tenant workshop management: vehicles, repair jobs, mechanics, invoices, and payments — one deployment serves many garages with fully isolated data per garage.

- **Tenancy by design** — every garage gets isolated tables of data, its own invoice/quote number sequences, and a garage code required at login; a super-admin panel manages garages (create, disable, delete-with-confirmation)
- **Repair workflow as a state machine** — Awaiting Diagnosis → … → Fixed / Unable to Fix, with full status history, odometer-based service logging, and mechanic "My Jobs" views
- **Invoicing built real** — pdfkit PDF invoices and payment receipts, quotations via WhatsApp approval, parts stock that deducts/restores and raises low-stock alerts; runs with Docker Compose in one command

`React (Vite + Tailwind) · Node.js · Express · MySQL · JWT + bcrypt · pdfkit · Docker`

### 3. [AI Learns to Drive](https://github.com/ARTI-INTEL/AI-Learns-to-Drive)
A reinforcement-learning study in autonomy: a car teaches itself to drive a race track with NEAT neuroevolution — no training data, no human demonstrations.

- NEAT evolves **both weights and network topology** across generations, with speciation and checkpoint-based fitness (+200 per checkpoint, +500 per lap)
- 7 ray-cast sensors plus speed feed a network that decides steering and throttle; collision detection, real-time visualization, and a waypoint track editor drawn from scratch
- Interactive, demo, and headless training modes for 10–50× faster evolution, with resumable checkpoints every generation

`Python · NEAT-Python · pygame`

### 4. [Handwritten Character Recognition](https://github.com/ARTI-INTEL/Handwritten-Character-Recognition)
A CNN ablation study: what does each architectural change *actually* buy? Built on MNIST and EMNIST-Balanced, measured the same way at every rung.

- Ten-rung ladder from logistic regression to a residual CNN, where each rung differs by exactly one change — and deliberately separates "deeper" from "bigger" with a parameter-matched wide net
- Verified the torchvision **EMNIST orientation trap empirically** with a transfer probe (a wrong transform costs >30 accuracy points); the correct fix was measured, not copied
- Honest methodology throughout: CPU-only reproducible inference timing (latency at batch 1/32/256), touched-twice test protocol, structured error analysis

`Python · PyTorch · torchvision`

### 5. [Credit Scoring Model](https://github.com/ARTI-INTEL/Credit-Scoring-Model)
Creditworthiness prediction on the UCI German Credit dataset that optimizes for **financial cost**, not just accuracy.

- Benchmarked Logistic Regression, Random Forest, LightGBM, and XGBoost under identical preprocessing, with class-weighting and asymmetric-cost thresholding (defaults weighted 5× false approvals)
- Cut total modeled financial loss from 149 → 95 cost units (ROC-AUC 0.794–0.809) while lifting default recall to 80%
- Delivered as a reproducible Jupyter notebook plus a one-page executive summary for non-technical stakeholders

`Python · scikit-learn · LightGBM · XGBoost · pandas · Jupyter`

### Also on GitHub

| Repository | What it is |
|---|---|
| [24AM-Radar-Published](https://github.com/ARTI-INTEL/24AM-Radar-Published) | Full-stack flight-tracking app (OpenSky API, Leaflet.js, MySQL, auth) — graded-unit (GU2) assessment |
| [Astro-Tracker](https://github.com/ARTI-INTEL/Astro-Tracker) · [Live demo](https://arti-intel.github.io/Astro-Tracker/) | Health-tracking web app (sleep, workouts, diet) + packaged Android APK |
| [Dubai-Tour-Site](https://github.com/ARTI-INTEL/Dubai-Tour-Site) · [Live demo](https://arti-intel.github.io/Dubai-Tour-Site/) | Responsive tourism site for Dubai & UAE attractions |
| [fr-ml-intern-starter](https://github.com/ARTI-INTEL/fr-ml-intern-starter) | FlyRank Machine Learning Internship repository |

---

## Tech stack

Technologies below appear in my deployed projects, public repositories, or verified course work. Things I'm currently learning are labeled as such.

**Languages**

![JavaScript](https://img.shields.io/badge/JavaScript-10223F?style=flat-square&logo=javascript&logoColor=white)
![Python](https://img.shields.io/badge/Python-10223F?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-10223F?style=flat-square&logo=Java&logoColor=white)
![C%2B%2B](https://img.shields.io/badge/C%2B%2B-10223F?style=flat-square&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-10223F?style=flat-square&logoColor=white)
![VB.NET](https://img.shields.io/badge/VB.NET-10223F?style=flat-square&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-10223F?style=flat-square&logo=react&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-10223F?style=flat-square&logo=vite&logoColor=white)
![Tailwind%20CSS](https://img.shields.io/badge/Tailwind%20CSS-10223F?style=flat-square&logo=tailwindcss&logoColor=white)
![HTML%2FCSS](https://img.shields.io/badge/HTML%2FCSS-10223F?style=flat-square&logoColor=white)
![Leaflet.js](https://img.shields.io/badge/Leaflet.js-10223F?style=flat-square&logoColor=white)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-10223F?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-10223F?style=flat-square&logo=express&logoColor=white)
![REST%20APIs](https://img.shields.io/badge/REST%20APIs-10223F?style=flat-square&logoColor=white)
![JWT%20Auth](https://img.shields.io/badge/JWT%20Auth-10223F?style=flat-square&logo=jsonwebtokens&logoColor=white)
![WebRTC%20%2F%20WebSocket](https://img.shields.io/badge/WebRTC%20%2F%20WebSocket-10223F?style=flat-square&logoColor=white)

**Databases**

![MySQL](https://img.shields.io/badge/MySQL-10223F?style=flat-square&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-10223F?style=flat-square&logo=sqlite&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-10223F?style=flat-square&logo=mongodb&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-10223F?style=flat-square&logo=pytorch&logoColor=white)
![scikit--learn](https://img.shields.io/badge/scikit--learn-10223F?style=flat-square&logo=scikitlearn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-10223F?style=flat-square&logo=pandas&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-10223F?style=flat-square&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-10223F?style=flat-square&logoColor=white)
![NEAT--Python](https://img.shields.io/badge/NEAT--Python-10223F?style=flat-square&logoColor=white)

**DevOps & Cloud**

![Docker](https://img.shields.io/badge/Docker-10223F?style=flat-square&logo=docker&logoColor=white)
![Git%20%2F%20GitHub](https://img.shields.io/badge/Git%20%2F%20GitHub-10223F?style=flat-square&logo=git&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-10223F?style=flat-square&logo=netlify&logoColor=white)
![Render](https://img.shields.io/badge/Render-10223F?style=flat-square&logo=render&logoColor=white)
![GitHub%20Pages](https://img.shields.io/badge/GitHub%20Pages-10223F?style=flat-square&logo=github&logoColor=white)

**Learning next:** Next.js · TypeScript · CI/CD · deeper cloud deployment

---

## Experience & learning

**Machine Learning Intern @ FlyRank AI** · Jun – Sep 2026
Designed, trained, and evaluated ML models on real datasets — dataset exploration, feature engineering, model optimization, and performance analysis. Capstone project reviewed and accepted.

**Machine Learning Intern @ AgenticX AI Lab** · Sep – Oct 2026
Supervised-learning fundamentals with the emphasis on what makes a model useful: honest validation, class imbalance, feature leakage, and metrics matched to the business question.

**Training**
- Google — *Introduction to Large Language Models* & *Introduction to Reliable Deep Learning* (2026)
- Anthropic — *AI Fluency* series, MCP, Claude Code, and agent-skills courses (2026)
- Foundation courses — Python advanced programming, JavaScript advanced, C++ advanced, HTML/CSS

**Competitions** — NASA Space Apps Challenge 2025 (participant); robotics competition, 2nd place; Texpo programming competition, 3rd place

---

## GitHub activity

<!-- Rendered by maintained services (github-readme-stats, github-readme-streak-stats); the profile reads fine without them. -->

<a href="https://github.com/anuraghazra/github-readme-stats">
  <img src="https://github-readme-stats.vercel.app/api?username=ARTI-INTEL&show_icons=true&include_all_commits=true&theme=tokyonight&hide_border=true" alt="GitHub statistics for ARTI-INTEL: commits, pull requests, and repository counts" width="49%"/>
</a>
<a href="https://github.com/anuraghazra/github-readme-stats">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ARTI-INTEL&layout=compact&theme=tokyonight&hide_border=true" alt="Most used languages across ARTI-INTEL's public repositories" width="49%"/>
</a>
<a href="https://github.com/denvercoder1/github-readme-streak-stats">
  <img src="https://streak-stats.demolab.com?user=ARTI-INTEL&hide_border=true&locale=en" alt="ARTI-INTEL's current and longest GitHub contribution streak" width="63%"/>
</a>

---

## Connect

- **Portfolio:** [faiqimranportfolio.netlify.app](https://faiqimranportfolio.netlify.app/)
- **GitHub:** [github.com/ARTI-INTEL](https://github.com/ARTI-INTEL)
- **LinkedIn:** [Muhammad Faiq Imran](https://www.linkedin.com/in/muhammad-faiq-imran-99665a308/)
- **Email:** [faiqimran.fi@gmail.com](mailto:faiqimran.fi@gmail.com)

---

*Good software solves a real workflow; good ML solves it honestly. I build both, one schema and one metric at a time — on the way to systems that earn the word "intelligent".*

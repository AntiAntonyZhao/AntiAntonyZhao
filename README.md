# Hi, I'm Antony (Anti) Zhao 👋

**Software Engineer · AI / RAG · Full-Stack** · McGill Software Engineering, Class of 2026 · Montréal

I build LLM-powered tools and the full-stack systems that ship them: retrieval pipelines grounded in real data, React/TypeScript frontends, Python and Java backends, and CI/CD on the cloud. Previously interned at **SAP**, **MiniMax AI**, and **LONGi Solar**.

**📌 Open to new-grad full-time software & AI engineering roles — Montréal / Toronto.**

[Portfolio & résumé](https://antony-portfolio-509301.web.app/) · [LinkedIn](https://www.linkedin.com/in/antony-anti-zhao-0b7774222/) · [Email](mailto:anti.zhao@mail.mcgill.ca)

---

## 🌟 Featured projects

### 🤖 Portfolio site with a RAG career assistant · [live demo](https://antony-portfolio-509301.web.app/)
A recruiter-facing chatbot that answers questions about my background, grounded in a structured experience corpus so it doesn't make up answers.
- **Stack:** React + TypeScript on Firebase Hosting · FastAPI in a container on Cloud Run · ChromaDB · OpenAI API
- **Shipping:** push-to-deploy with GitHub Actions and Workload Identity Federation, so CI holds no long-lived service-account keys
- **Hardening:** API keys injected from Secret Manager, per-IP rate limiting, and request input caps against credential leaks and runaway API spend

### 🔎 Prospect — LLM job-posting extraction & résumé tailoring · 🚧 in progress
A pipeline I'm building for my own job search. What it's designed to do:
- Pull postings from public ATS job-board APIs (Greenhouse, Lever, Ashby) into SQLite, with content-hash deduplication to flag reposts
- Extract structured fields with tiered model routing (Haiku → Sonnet → Opus) to trade cost against accuracy
- Tailor résumé bullets from a YAML/Pydantic fact bank under a no-fabrication rule: the model may only select and rephrase facts that exist in the bank
- Built agent-first with Claude Code against a `CLAUDE.md` spec, with integrity rules encoded as pytest checks and PreToolUse hooks so agent-written code can't bypass them

## 🧩 More projects

| Project | Highlights | Code |
|---|---|---|
| **Mosaic** — local LLM desktop app (8-person team) | Llama 3B-Instruct running offline with hot-swappable qLoRA adapters. My part: SQLite schema with crash-safe writes, Java ↔ FastAPI/llama.cpp integration over REST, and the Application component's UML domain model | on request |
| **Ataxx game agent** | Minimax with alpha-beta pruning and iterative deepening under a 2-second move limit; a transposition table cut computation ~50%. 91.3% win rate vs. heuristic agents, 93.5% vs. MCTS agents | on request |
| **Inventory system + DevOps pipeline** | Spring Boot + React app deployed on Azure, with build, test, and deployment automated through Azure DevOps and Docker | [repo](https://github.com/AntiAntonyZhao/E437Final) |
| **Applied ML projects** | Linear/logistic regression from scratch; MLP vs. CNN (74.43% → 83.88%); Naive Bayes vs. fine-tuned BERT for emotion classification (76.55% → 93%) | [repo](https://github.com/AntiAntonyZhao/MachineLearning) |
| **REST API validation** | Exploratory, story-based, and performance testing of a REST API with PyTest and Cucumber; surfaced undocumented behaviour and stability issues | [repo](https://github.com/AntiAntonyZhao/Software-Validation) |

## 💼 Experience

- **LONGi Solar North America** · Development Intern (part-time, remote) · Sep 2025 – Apr 2026  
  Integrated an LLM-powered search assistant into internal training sites, fixed frontend bugs, and supported end-to-end QA of the Canadian product site.
- **SAP** · iXp Intern · Montréal · Oct 2024 – May 2025  
  Built React/JavaScript features with permission-based filtering, real-time log streaming over WebSockets, and cloud automation tools for SAP Commerce Cloud; completed 105+ Agile work items and resolved 78+ production bugs.
- **MiniMax AI** · AI Operations Intern · Shanghai · May – Aug 2023  
  Designed a GPT-4 vs. MiniMax benchmarking pipeline across 50+ multi-turn dialogue scenarios, with Python automation for prompt execution and comparative scoring.

## 🛠️ Tech

- **Languages:** Python · Java · TypeScript · JavaScript · SQL · C · Bash
- **AI / LLM:** RAG · ChromaDB · OpenAI API · prompt engineering · LLM evaluation · PyTorch · Hugging Face Transformers · llama.cpp
- **Backend & frontend:** FastAPI · Spring Boot · REST · WebSockets · React
- **Cloud & DevOps:** Docker · GitHub Actions · Azure · Azure DevOps · Google Cloud (Cloud Run, Firebase Hosting, Secret Manager)
- **Data & testing:** SQLite · PostgreSQL · PyTest · JUnit · Cucumber
- **AI-assisted development:** Claude Code · Cursor · GitHub Copilot · OpenAI Codex

---

🏸 Off-screen: former McGill varsity badminton player.

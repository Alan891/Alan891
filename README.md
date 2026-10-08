<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="Alan Balcerowiak — AI Solutions Engineer. RAG that says “I don't know” by design." src="assets/banner-light.svg" width="100%">
</picture>

<p>
  <a href="https://alanbalcerowiak.pl"><img alt="Website" src="https://img.shields.io/badge/alanbalcerowiak.pl-17150f?style=flat-square&logo=googlechrome&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/alan-balcerowiak/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="mailto:contact@alanbalcerowiak.pl"><img alt="Email" src="https://img.shields.io/badge/contact@alanbalcerowiak.pl-c2410c?style=flat-square&logo=maildotru&logoColor=white"></a>
</p>

I design and ship **on-premise LLM and RAG systems** on the Polish model **Bielik**, so company data never leaves its own infrastructure.

> **RAG that refuses.** “Answer only from the context” works in roughly 80% of cases. The other 20% is a hallucination that ends up as a screenshot in the company Slack. In my systems, *“I don't know”* is enforced by architecture: a relevance filter before the model is called and a separate decision layer, not a line in the prompt.

### What I work on

| | |
|---|---|
| **On-prem RAG** | Answers grounded in company documents, with cited sources and enforced refusal |
| **Tool-calling assistants** | Answers built from tool results, read-only enforced by design |
| **AI for network security** | Deterministic configuration analysis, explained in natural language |
| **Brand-style image generation** | LoRA fine-tuning, tenant isolation, RBAC |
| **Voice assistants** | Whisper → LLM → Piper on a single GPU |

Second track: **AI-augmented security research**: testing web applications with AI (recon, fuzzing, payload generation) and reporting directly to security teams.

### Stack

![Bielik](https://img.shields.io/badge/Bielik-LLM-17150f?style=flat-square)
![vLLM](https://img.shields.io/badge/vLLM-serving-17150f?style=flat-square)
![BGE-M3](https://img.shields.io/badge/BGE--M3-embeddings-17150f?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-vector%20DB-17150f?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Whisper](https://img.shields.io/badge/Whisper-speech-17150f?style=flat-square)
![LoRA](https://img.shields.io/badge/LoRA-fine--tuning-17150f?style=flat-square)

### How I work

1. I use a tool myself, every day, on real data, before it reaches a client.
2. *“I don't know”* is a valid answer. Better to refuse once than to lie once.
3. The best technology is the one the user never has to think about.

<sub>🇵🇱 Inżynier Rozwiązań AI z Krakowa. Lokalne systemy LLM i RAG na Bieliku, w których „nie wiem” wymusza architektura, a nie prompt. Więcej po polsku: <a href="https://alanbalcerowiak.pl">alanbalcerowiak.pl</a></sub>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="Alan Balcerowiak — AI Solutions Engineer" src="assets/banner-light.svg" width="100%">
</picture>

<h3>I build RAG that says <i>“I don't know”</i> — enforced by architecture, not by the prompt.</h3>

<p>On-premise LLM systems on the Polish model <b>Bielik</b> · company data never leaves its own infrastructure · Kraków, Poland</p>

[![Typing SVG](https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=19&duration=2800&pause=900&color=C2410C&center=true&vCenter=true&width=720&height=40&lines=On-prem+RAG+with+enforced+refusal;Bielik+%C2%B7+vLLM+%C2%B7+BGE-M3+%C2%B7+ChromaDB+%C2%B7+FastAPI;Tool-calling+assistants%2C+read-only+by+design;Voice%3A+Whisper+%E2%86%92+LLM+%E2%86%92+Piper+on+one+GPU;AI-augmented+security+research)](https://alanbalcerowiak.pl)

<p>
<a href="https://alanbalcerowiak.pl"><img src="https://img.shields.io/badge/Portfolio-alanbalcerowiak.pl-c2410c?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
<a href="https://www.linkedin.com/in/alan-balcerowiak/"><img src="https://img.shields.io/badge/LinkedIn-Alan%20Balcerowiak-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:contact@alanbalcerowiak.pl"><img src="https://img.shields.io/badge/Email-contact@alanbalcerowiak.pl-17150f?style=for-the-badge&logo=maildotru&logoColor=white" alt="Email"/></a>
</p>

<img src="https://komarev.com/ghpvc/?username=Alan891&label=Profile%20views&color=c2410c&style=flat-square" alt="Profile views"/>

</div>

---

## 🧭 At a glance

| | Details |
|---|---|
| **Role** | AI Solutions Engineer — architecture to production for on-premise LLM products |
| **Focus** | Private RAG on company documents · tool-calling assistants · voice AI · AI for security |
| **Signature idea** | *“I don't know”* as a first-class answer: relevance filter + decision layer **before** the model is called |
| **Second track** | AI-augmented security research with direct, responsible disclosure |
| **Studying** | Cybersecurity, Andrzej Frycz Modrzewski Kraków University (2025–2028) |
| **Certified** | Generative AI with Large Language Models — DeepLearning.AI × AWS (2026) |
| **Based in** | Kraków, Poland · 🇵🇱 Polish · 🇬🇧 English · 🇩🇪 German (basic) |

---

## 📊 In numbers

<table align="center">
<tr>
<td align="center" width="20%"><img src="https://img.icons8.com/fluency/96/server.png" width="44"/><br><b>100%</b><br>on-premise</td>
<td align="center" width="20%"><img src="https://img.icons8.com/fluency/96/artificial-intelligence.png" width="44"/><br><b>5</b><br>solution areas</td>
<td align="center" width="20%"><img src="https://img.icons8.com/fluency/96/rocket.png" width="44"/><br><b>14</b><br>web products shipped solo</td>
<td align="center" width="20%"><img src="https://img.icons8.com/fluency/96/bug.png" width="44"/><br><b>5</b><br>vulnerabilities reported &amp; patched</td>
<td align="center" width="20%"><img src="https://img.icons8.com/fluency/96/cloud-cross.png" width="44"/><br><b>0</b><br>data sent to third-party clouds</td>
</tr>
</table>

---

## 🧠 RAG that refuses

> “Answer only from the context” works in roughly **80%** of cases. The other 20% is a hallucination that lands in the company Slack as a screenshot. So the decision *answer vs. refuse* is made **before** the LLM ever sees the question.

```mermaid
flowchart LR
    Q([User question]) --> E[BGE-M3<br/>embeddings]
    E --> R[(ChromaDB<br/>retrieval)]
    R --> F{Relevance<br/>filter}
    F -- "close, but not about it" --> X([“I don't know”])
    F -- relevant --> D{Decision<br/>layer}
    D -- refuse --> X
    D -- answer --> L[Bielik on vLLM]
    L --> A([Answer + cited sources])
    style X fill:#c2410c,color:#fff,stroke:#c2410c
    style A fill:#17150f,color:#f3efe6,stroke:#17150f
    style L fill:#f3efe6,stroke:#17150f
```

**How I measure it:** regression tests — out of 100 questions *outside* the knowledge base, how many end in a refusal.

---

## 🛠️ What I work on

| Area | Approach | Typical stack |
|---|---|---|
| **On-prem RAG** | Grounded answers with cited sources; refusal enforced by architecture | Bielik · vLLM · BGE-M3 · ChromaDB · FastAPI |
| **Tool-calling assistants** | The model answers from tool results, not memory; read-only enforced by design | Bielik · tool calling · Python · FastAPI |
| **AI for network security** | Deterministic configuration analysis, explained by an LLM in plain language | Python · static analysis · Bielik |
| **Brand-style image generation** | LoRA fine-tuning, tenant isolation, access control | Python · LoRA · RBAC · multi-tenancy |
| **Voice assistants** | Speech → model → speech in one pipeline, nothing leaves the box | Whisper · Bielik · Piper · vLLM |

---

## 🧰 Tech stack

**Models & serving**

![Bielik](https://img.shields.io/badge/Bielik-Polish_LLM-c2410c?style=for-the-badge)
![vLLM](https://img.shields.io/badge/vLLM-serving-17150f?style=for-the-badge)
![Whisper](https://img.shields.io/badge/Whisper-speech--to--text-17150f?style=for-the-badge)
![Piper](https://img.shields.io/badge/Piper-text--to--speech-17150f?style=for-the-badge)
![LoRA](https://img.shields.io/badge/LoRA-fine--tuning-17150f?style=for-the-badge)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=000000)

**Retrieval & data**

![BGE-M3](https://img.shields.io/badge/BGE--M3-embeddings-3b1d0e?style=for-the-badge)
![ChromaDB](https://img.shields.io/badge/ChromaDB-vector_DB-3b1d0e?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-with_refusal-3b1d0e?style=for-the-badge)
![Tool calling](https://img.shields.io/badge/Tool_calling-read--only-3b1d0e?style=for-the-badge)

**Apps, APIs & infra**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=000000)
![GPU](https://img.shields.io/badge/Own_GPU-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

**Security**

![AppSec](https://img.shields.io/badge/Web_AppSec-17150f?style=for-the-badge&logo=owasp&logoColor=white)
![Pentesting](https://img.shields.io/badge/Penetration_testing-17150f?style=for-the-badge)
![Network security](https://img.shields.io/badge/Network_security-17150f?style=for-the-badge)
![RBAC](https://img.shields.io/badge/RBAC_·_multi--tenancy-17150f?style=for-the-badge)

---

## 🔐 AI-augmented security research

I test web applications with AI in the loop and report findings **directly** to the teams that own them — no bug-bounty middlemen. So far: **5 vulnerabilities** reported in one application, including **one critical**; the team paid a bounty and **all were patched**.

---

## 🧭 How I work

1. **I use the tool myself first** — every day, on real data — before it reaches a client.
2. **“I don't know” is a valid answer.** Better to refuse once than to lie once.
3. **The best technology is the one the user never has to think about.**

---

<div align="center">

**Need a private AI assistant that runs on your own hardware and knows when to say “I don't know”?**

<a href="mailto:contact@alanbalcerowiak.pl"><img src="https://img.shields.io/badge/Let's_talk-contact@alanbalcerowiak.pl-c2410c?style=for-the-badge&logo=maildotru&logoColor=white" alt="Let's talk"/></a>

<sub>🇵🇱 Inżynier Rozwiązań AI z Krakowa — więcej po polsku na <a href="https://alanbalcerowiak.pl">alanbalcerowiak.pl</a></sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:c2410c,45:3b1d0e,100:17150f&height=110&section=footer" width="100%" alt=""/>

</div>

# Aditya Sharma

**Senior AI Engineer at Savills** — I build agent systems that survive production.

Mathematics degree first; agents since 2024, before the hype. Savills was my client at
Datasmith — then they hired me.

**[→ neural chalchitra, my portfolio](https://adityaa-sharma.github.io/neural-chalchitra/)** —
every project as a star: read it as an index, or take the 3D flight through it.

---

## Numbers I stand behind

| number | where it comes from |
|-------:|---------------------|
| **< 4 s** | agent latency — 8 tools on a 16k context. MHADA (Govt. of Maharashtra), live at mhada.gov.in, answering in Marathi |
| **100+** | concurrent users — 4×A100 80GB, model parallelism + round-robin. I deployed the whole estate: vLLM, Whisper, TTS, vision, Redis, Celery, Postgres, across prod/UAT/dev |
| **10,000** | leases keyword-extracted in one pass — Ray, one model sharded across 4 VMs |
| **8B** | Qwen3-VL fine-tuned (LoRA SFT → GRPO, reward functions I wrote myself) past the closed models on valve-industry datasheets |

## Where that happened

**Savills** — Senior AI Engineer, 2025 — present. They were my client across 22 APAC
business lines; when I was leaving Datasmith, they offered me the role. Architected the
APAC agent platform — agents, schedulers, outputs as live React components — and demoed
it to the APAC CIO. Worked GST/TDS reconciliation through with the India CFO, built an
RFI-response generator over SharePoint, led hiring for the AI team.

**Datasmith.ai** — Founding member, 2024 — 2025. Owned client work from POC to
production: MHADA (the agent above), TenderGenie (the fine-tune above, shipped during my
notice period), and AI Lake — chat with all your data (CSV, Postgres, Mongo), the agent
choosing which React component to answer with, a knowledge graph underneath.

**PG-AGI** — AI/ML Intern, 2024. Chat-with-database on OpenAI function calling + DSPy,
built to sit under voice agents — before "agentic" was a pitch-deck word.

**Freelance, live today** — [eve](https://eve2-frontend-62944796586.us-central1.run.app/en-US/):
university search on parent-child RAG (a school can have 400+ programs; one chunk cannot
hold them), Airflow ingestion. [latimer.ai](https://www.latimer.ai/): chat, auth, magic links.

**Before all of it** — B.S. Honors Mathematics, then M.S. AI & ML at IIIT Lucknow
(9.23 CGPA). The math came first on purpose.

## Independent research — the part that's public

The production work above is closed-source, so what you can read here is the
foundational side: papers implemented from scratch, and the layers under the frameworks.

| repo | what it is |
|------|------------|
| [GPT-2-Scratch](https://github.com/Adityaa-Sharma/GPT-2-Scratch) | GPT-2 built from the paper — 21.77M params, character-level, trained on 11k poems on a single 16GB T4 |
| [Linformer-paper-implemetation](https://github.com/Adityaa-Sharma/Linformer-paper-implemetation) | Linformer from the paper — attention from O(N²) to O(N) |
| [DeepQlearning](https://github.com/Adityaa-Sharma/DeepQlearning) | DeepMind's DQN — my agent plays Atari Breakout after ~1,600 episodes |
| [cudaKernels](https://github.com/Adityaa-Sharma/cudaKernels) | going below the framework, one kernel at a time |
| [Trading_mcp_server](https://github.com/Adityaa-Sharma/Trading_mcp_server) | an MCP server that gives LLMs real hands — live Upstox portfolio, order execution ([demo](https://www.loom.com/share/11669cb8a1ad4867971af8f6b9b8516c)) |
| [Ref_Reader_Backend](https://github.com/Adityaa-Sharma/Ref_Reader_Backend) | ArXiv research assistant — two-stage RAG, Qdrant + Postgres, deployed |

## Stack I actually use

- **Serving & infra** — vLLM · Ray · Docker · Redis · Celery · Postgres · Airflow · Superset
- **Training** — PyTorch · TRL (SFT, GRPO) · LoRA · Weights & Biases · AWQ quantisation
- **Agents & retrieval** — function calling · MCP · DSPy · Qdrant · Neo4j · parent-child RAG
- **Learning right now** — CUDA kernels · vLLM internals · React (the portfolio is my JS classroom)

## Problems I'm chasing

Context bloat — most "hallucinations" I have debugged were context problems; MHADA runs
on a 16k window on purpose. Hallucination control you can grade with a reward function.
And the standing rule of production ML: one box is never the final answer.

## Reach me

[adityasharma.jprr@gmail.com](mailto:adityasharma.jprr@gmail.com) ·
[portfolio](https://adityaa-sharma.github.io/neural-chalchitra/) ·
[linkedin](https://www.linkedin.com/in/aditya-jpr/) ·
[hugging face](https://huggingface.co/Adityyaa)

फिर मिलेंगे — *see you around.*

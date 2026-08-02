# Aditya Sharma

**I build agent systems that survive production.**

Mathematics degree → models → the machines they run on. Python and PyTorch first;
when a thing doesn't make sense from the outside, I reimplement the paper.

**[→ neural chalchitra, my portfolio](https://adityaa-sharma.github.io/neural-chalchitra/)** —
every project as a star: read it as an index, or take the 3D flight through it.

---

## Things I've built

- **An 8-tool agent on a government portal**, answering in Marathi — under **4 s** on a
  16k context, kept small on purpose: most "hallucinations" I have debugged were
  context problems.
- **A vision-model fine-tune that beat the closed models** on industrial datasheets —
  Qwen3-VL-8B, LoRA SFT → GRPO with reward functions I wrote myself: JSON validity,
  schema compliance, per-field accuracy, a hallucination penalty.
- **A full serving estate** — vLLM + Whisper + TTS + vision on 4×A100 80GB, model
  parallelism + round-robin for **100+ concurrent users**, prod/UAT/dev, deployed
  end to end by me.
- **A one-pass extraction over 10,000 leases** — one model sharded across 4 VMs
  with Ray.
- **Chat with all your data** — CSV, Postgres, Mongo behind one agent that chooses
  which React component to answer with, a knowledge graph underneath.
- **Agents with real hands** — an MCP server doing live portfolio reads and order
  execution from the editor, and chat-with-database on function calling + DSPy back
  in 2024, before "agentic" was a pitch-deck word.

*Built at Savills (current), Datasmith.ai, and PG-AGI —
[the full stories, in order](https://adityaa-sharma.github.io/neural-chalchitra/).*

## Public work

The production systems above are closed-source; what you can read here is the
foundational side — papers implemented from scratch, and the layers under the frameworks.

| repo | what it is |
|------|------------|
| [GPT-2-Scratch](https://github.com/Adityaa-Sharma/GPT-2-Scratch) | GPT-2 built from the paper — 21.77M params, character-level, trained on 11k poems on a single 16GB T4 |
| [Linformer-paper-implemetation](https://github.com/Adityaa-Sharma/Linformer-paper-implemetation) | Linformer from the paper — attention from O(N²) to O(N) |
| [DeepQlearning](https://github.com/Adityaa-Sharma/DeepQlearning) | DeepMind's DQN — my agent plays Atari Breakout after ~1,600 episodes |
| [cudaKernels](https://github.com/Adityaa-Sharma/cudaKernels) | going below the framework, one kernel at a time |
| [Trading_mcp_server](https://github.com/Adityaa-Sharma/Trading_mcp_server) | an MCP server that gives LLMs real hands — live Upstox portfolio, order execution ([demo](https://www.loom.com/share/11669cb8a1ad4867971af8f6b9b8516c)) |
| [Ref_Reader_Backend](https://github.com/Adityaa-Sharma/Ref_Reader_Backend) | ArXiv research assistant — two-stage RAG, Qdrant + Postgres, deployed |

## Stack

- **Languages** — Python (first language) · C++ · SQL · TypeScript (learning, in public)
- **Training** — PyTorch · TRL (SFT, GRPO) · LoRA / PEFT · Weights & Biases · AWQ quantisation
- **Serving & distributed** — vLLM · Ray · FastAPI · Docker · Redis · Celery · Postgres · Airflow · Superset
- **Agents & retrieval** — MCP · function calling · DSPy · Qdrant · Neo4j · Whisper / TTS
- **Below the framework** — CUDA kernels · vLLM internals — reading the engine I deploy

## What I want to work on

Context engineering — bloat is the real enemy, and small windows are a feature.
Hallucination control you can grade with a reward function instead of a vibe.
Serving efficiency, because one box is never the final answer. And on the
foundational side: papers from scratch — attention, Linformer, DQN so far — with
CUDA next. I want problems where the math has to survive contact with production.

## Reach me

[adityasharma.jprr@gmail.com](mailto:adityasharma.jprr@gmail.com) ·
[portfolio](https://adityaa-sharma.github.io/neural-chalchitra/) ·
[linkedin](https://www.linkedin.com/in/aditya-jpr/) ·
[hugging face](https://huggingface.co/Adityyaa)

फिर मिलेंगे — *see you around.*

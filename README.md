<div align="center">

# MaaS-YT

### The companion to my YouTube channel — where we take on real engineering challenges.

*I study how machines learn. I build systems that actually do.*

**Build it. Break it. Measure it. Understand it. Improve it.**

[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-FF0000?style=for-the-badge&logo=youtube)](https://youtube.com/playlist?list=PLVM9Nqm8zLE0)
[![Portfolio](https://img.shields.io/badge/Portfolio-B45309?style=for-the-badge)](https://silvaxxx1.github.io/MyWebsite/)
[![SAiR](https://img.shields.io/badge/SAiR_Org-181717?style=for-the-badge)](https://github.com/SAIR-Org)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/mohammed-sedeg-67444b307/)

</div>

---

## 👋 Who's Behind This

I'm **Mohammed "Silva" Sedeg** — an AI Systems Engineer working across LLMs, edge AI, and MLOps, and a PhD candidate at Karabük University researching vision-language models and model optimization for constrained hardware.

Before AI, I spent years running **PLC/HMI/SCADA** systems and building physical infrastructure — solar trackers, automation lines, hybrid solar-EV systems. That background shapes how I approach software now: I want to know what's happening at the layer underneath, not just how to call the API.

I also founded **[SAiR](https://github.com/SAIR-Org)** (سير — "walking on a road"), a free, project-based AI education org that started in Sudan and is now open to learners across Africa, the Middle East, and the Global South. 200+ students have gone through it, and the flagship cohort didn't just learn attention mechanisms from a slide — they built **[miniGPT](https://github.com/SAIR-Org/miniGPT)**, a full GPT trained and served end-to-end, from tokenizer to web UI, with 39 passing tests.

That's the same standard this channel holds itself to: don't just explain the concept, ship the working system. This org is where I document that process for MLOps, inference engines, and Python internals.

> **Full background, production numbers, and project list → [my portfolio](https://silvaxxx1.github.io/MyWebsite/)**

---

## 🎥 What You'll Find Here

The material covers the engineering layers behind modern AI systems:

```text
Python
   ↓
Machine Learning
   ↓
Deep Learning
   ↓
MLOps
   ↓
Model Serving
   ↓
Inference Engineering
   ↓
Systems
   ↓
Hardware
```

The goal isn't to cover everything. It's to go deep enough into a problem to understand **what is actually happening underneath the abstraction**.

---

## 🔥 Current Challenge

### MLOps from First Principles
**Status: 🟢 Complete**

We started with a practical question:

> **You have a machine learning model. How do you turn it into a production system?**

Instead of jumping straight into tools, the series builds the system layer by layer.

```text
Model → Serving → Reproducibility → Data Engineering
      → Model Optimization → Cloud Infrastructure → Observability
```

| Module | Challenge                                 | Technologies                                                  |
| ------ | ------------------------------------------ | --------------------------------------------------------------- |
| **01** | How does anything call the model?          | FastAPI, Docker                                                  |
| **02** | How do we reproduce experiments?           | Git, DVC, MLflow, W&B                                            |
| **03** | How does data reach the model?             | Feast, Prefect, Spark                                            |
| **04** | How do we make models smaller and faster?  | Pruning, Quantization, KD, ONNX, TorchScript, LibTorch, gRPC     |
| **05** | How do we run this in production?          | Kubernetes, AWS, EKS                                             |
| **06** | How do we know the system is degrading?    | Evidently, Prometheus, Grafana                                   |

**Repo:** [MLOps from First Principles](https://github.com/MaaS-YT/MLOps-from-the-first-principles)
**Playlist:** [Watch on YouTube](https://youtube.com/playlist?list=PLVM9Nqm8zLE0)

---

## 🚧 What's Next

### ⚡ Head First into Inference Engineering
**Status: 🟡 In Development**

I've spent real time building on top of **vLLM** and **SGLang** in production — but using the abstraction only gets you so far. This series goes underneath it.

Studying through *Inference Engineering*, *Fast & Efficient LLM Inference with vLLM*, *Efficient Inference with SGLang*, and *Fast LLM Inference with Cerebras* — but the goal isn't to summarize them. The work is:

```text
Study → Implement → Benchmark → Profile → Optimize → Benchmark again → Understand why
```

Topics on deck: prefill vs. decode, KV cache, continuous batching, scheduling, memory bandwidth, GPU utilization, latency, throughput, quantization, kernel efficiency, and hardware/software interaction.

> **The central question: why is an inference system fast? Not: how do I call an inference API?**

This builds directly on production work I've shipped — including ~3× faster LLM inference via GGUF/ExLlamaV2 quantization and a ~40% RAG latency reduction through pipeline optimization. Now we go build and benchmark that from the ground up, on camera.

---

### 🐍 Python Mastery Hub
**Status: 🟡 In Development**

> **Can I actually use Python as a systems engineering tool?**

Knowing syntax isn't the same as understanding Python deeply enough to build efficient, maintainable AI infrastructure.

```text
Data Model → Data Structures → Functions & Types → Iterators → NumPy
           → Compilation → Classes & Protocols → Concurrency → Async
           → Production AI Systems
```

Every concept ties back to real AI engineering: PyTorch tensors, Dataset/DataLoader, profiling, numerical computing, configuration systems, concurrency, inference services.

**Checkpoint projects:**
1. Dataset + DataLoader from scratch
2. NumPy minibatch trainer + Numba optimization
3. Tiny `nn.Module`-style API
4. FastAPI inference endpoint with a warm process pool

**Repo:** [Python Mastery Hub](https://github.com/MaaS-YT/python-mastery-hub)

---

## 📚 Current & Upcoming

| Project                                   | Focus                             | Status             |
| ------------------------------------------- | ------------------------------------ | --------------------- |
| **MLOps from First Principles**             | Production ML systems               | 🟢 Complete         |
| **Head First into Inference Engineering**   | LLM inference & performance         | 🟡 In Development   |
| **Python Mastery Hub**                      | Advanced Python for AI engineers    | 🟡 In Development   |
| **AI Systems Experiments**                  | Systems, performance & hardware     | 🔵 Future           |

---

## 🧪 How We Work

Every challenge follows the same loop:

```text
Problem → Understand → Build → Measure → Break → Optimize → Understand
```

These repos aren't just notes — they're **working records of the challenges**, built the same way I build things in production: MyTorch (a PyTorch-from-scratch framework going down to custom CUDA/Triton kernels), MyLLM (a full pretrain-to-RLHF pipeline), and a production RAG platform are all part of the same philosophy applied elsewhere. See them on [my GitHub](https://github.com/silvaxxx1).

---

## 🗺️ The Direction

```text
                 REAL CHALLENGES
                       │
          ┌────────────┼────────────┐
          ↓            ↓            ↓
       MLOps       Python       Inference
          │            │            │
          └────────────┼────────────┘
                       ↓
                  AI SYSTEMS
                       │
          ┌────────────┼────────────┐
          ↓            ↓            ↓
       Software      Models       Hardware
                       │
                       ↓
              Production Systems
```

The topics may change. The methodology stays the same:

> **Take a real problem. Go underneath the abstraction. Build something. Measure it. Understand it.**

---

## 🔗 Related Work

* **[SAiR Organization](https://github.com/SAIR-Org)** — free, project-based AI education, Sudan-founded and open to Africa, the Middle East, and the Global South
* **[miniGPT](https://github.com/SAIR-Org/miniGPT)** — SAiR's capstone: a GPT built, trained, and deployed from scratch by students
* **[SAiR Jr. Curriculum](https://github.com/SAIR-Org/SAIR_Jr)** — the full free course, from Python fundamentals to GPT from scratch

MaaS-YT is the companion space for the personal YouTube channel. Where SAiR teaches the fundamentals to people starting out, MaaS-YT is where I go past the fundamentals — into the harder, less-charted territory of inference engines and systems performance — and solve those problems in public, in detail.

---

## 🎬 Start Here

**[▶️ MLOps from First Principles](https://youtube.com/playlist?list=PLVM9Nqm8zLE0)** — start with the production ML system.

**Next up:** Head First into Inference Engineering — going underneath modern LLM inference.

**Building the foundation:** Python Mastery Hub — the Python depth serious AI engineering requires.

---

<div align="center">

> **We don't just learn the tools.**
> **We take on the problem, go underneath the abstraction, and figure out how it actually works.**

📬 [Email](mailto:silvapi1994@gmail.com) · [LinkedIn](https://www.linkedin.com/in/mohammed-sedeg-67444b307/) · [Portfolio](https://silvaxxx1.github.io/MyWebsite/) · [SAiR](https://t.me/+jPPlO6ZFDbtlYzU0)

</div>

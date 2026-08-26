# MaaS-YT

### The companion to my YouTube channel — where we take on real engineering challenges.

This organization contains the **code, experiments, notes, projects, and technical deep dives** behind my YouTube channel.

The channel is not built around simply explaining tools.

We take on real challenges:

> **Build it. Break it. Measure it. Understand it. Improve it.**

Sometimes that means building an MLOps system from scratch.

Sometimes it means going underneath an LLM inference engine to understand why it is fast.

Sometimes it means profiling Python, optimizing a workload, or understanding what is happening between the model, software, and hardware.

The repositories here are the **companion material** for those journeys.

---

# 🎥 What You Will Find Here

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

The objective is not to cover everything.

It is to go deep enough into a problem to understand **what is actually happening underneath the abstraction**.

---

# 🔥 Current Challenge

## MLOps from First Principles

**Status: 🟢 Complete**

We started with a practical question:

> **You have a machine learning model. How do you turn it into a production system?**

Instead of jumping directly into tools, the series builds the system layer by layer.

```text
Model
  ↓
Serving
  ↓
Reproducibility
  ↓
Data Engineering
  ↓
Model Optimization
  ↓
Cloud Infrastructure
  ↓
Observability
```

### What we built and explored

| Module | Challenge                                 | Technologies                                                 |
| ------ | ----------------------------------------- | ------------------------------------------------------------ |
| **01** | How does anything call the model?         | FastAPI, Docker                                              |
| **02** | How do we reproduce experiments?          | Git, DVC, MLflow, W&B                                        |
| **03** | How does data reach the model?            | Feast, Prefect, Spark                                        |
| **04** | How do we make models smaller and faster? | Pruning, Quantization, KD, ONNX, TorchScript, LibTorch, gRPC |
| **05** | How do we run this in production?         | Kubernetes, AWS, EKS                                         |
| **06** | How do we know the system is degrading?   | Evidently, Prometheus, Grafana                               |

### Companion repository

**[MLOps from First Principles](https://github.com/MaaS-YT/MLOps-from-the-first-principles)**

The repository contains the written material, diagrams, experiments, and references accompanying the videos.

### ▶️ Playlist

**[MLOps from First Principles](https://youtube.com/playlist?list=PLVM9Nqm8zLE0)**

---

# 🚧 What's Next

The next challenges move deeper into **AI systems**.

---

# ⚡ Head First into Inference Engineering

### Long-Format Technical Deep Dive

**Status: 🟡 In Development**

I've spent a lot of time working with **vLLM** and **SGLang**, building applications and systems on top of them.

But eventually you reach a point where using the abstraction isn't enough.

You want to know:

> **What is actually happening underneath?**

So this challenge is about going head first into **LLM inference engineering**.

I'm currently studying the subject through:

* *Inference Engineering*
* Fast & Efficient LLM Inference with vLLM
* Efficient Inference with SGLang
* Fast LLM Inference with Cerebras

But the goal is not to summarize any of them.

The real work is:

```text
Study
  ↓
Implement
  ↓
Benchmark
  ↓
Profile
  ↓
Optimize
  ↓
Benchmark again
  ↓
Understand why
```

We'll investigate things such as:

* Prefill vs. decode
* KV cache
* Continuous batching
* Scheduling
* Memory bandwidth
* GPU utilization
* Latency
* Throughput
* Quantization
* Kernel efficiency
* Inference architectures
* vLLM
* SGLang
* Hardware/software interaction

The central question is:

> **Why is an inference system fast?**

Not:

> **How do I call an inference API?**

---

# 🐍 Python Mastery Hub

### Advanced Python for AI Engineers

**Status: 🟡 In Development**

Another challenge is closer to the foundation:

> **Can I actually use Python as a systems engineering tool?**

Knowing Python syntax is not the same as understanding Python deeply enough to build efficient, maintainable AI infrastructure.

The curriculum goes from the Python data model toward:

```text
Data Model
    ↓
Data Structures
    ↓
Functions & Types
    ↓
Iterators
    ↓
NumPy
    ↓
Compilation
    ↓
Classes & Protocols
    ↓
Concurrency
    ↓
Async
    ↓
Production AI Systems
```

### The challenge

We don't stop at Python examples.

We connect Python concepts directly to AI engineering:

* PyTorch
* tensors
* Dataset / DataLoader
* profiling
* numerical computing
* configuration systems
* concurrency
* inference services

### Checkpoint projects

The curriculum will build:

1. Dataset + DataLoader from scratch
2. NumPy minibatch trainer + Numba optimization
3. Tiny `nn.Module`-style API
4. FastAPI inference endpoint with a warm process pool

### Companion repository

**[Python Mastery Hub](https://github.com/MaaS-YT/python-mastery-hub)**

---

# 🗺️ The Direction

These projects are not isolated courses.

They are steps toward a larger engineering question:

> **How do we build AI systems that are actually fast, reliable, scalable, and understandable?**

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

The topics may change.

The methodology stays the same:

> **Take a real problem. Go underneath the abstraction. Build something. Measure it. Understand it.**

---

# 🧪 How We Work

Every challenge follows roughly the same loop:

```text
                 ┌──────────────┐
                 │    Problem   │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   Understand │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │     Build    │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   Measure    │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │    Break     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   Optimize   │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │  Understand  │
                 └──────────────┘
```

This means the repositories are not just collections of notes.

They are **working records of the challenges**.

---

# 📚 Current & Upcoming

| Project                                   | Focus                            | Status            |
| ----------------------------------------- | -------------------------------- | ----------------- |
| **MLOps from First Principles**           | Production ML systems            | 🟢 Complete       |
| **Head First into Inference Engineering** | LLM inference & performance      | 🟡 In Development |
| **Python Mastery Hub**                    | Advanced Python for AI engineers | 🟡 In Development |
| **AI Systems Experiments**                | Systems, performance & hardware  | 🔵 Future         |

---

# 🔗 Related Work

Some challenges connect to the broader SAiR learning ecosystem:

* **[SAiR Organization](https://github.com/SAIR-Org)**
* **[SAiR MLOps Blueprint](https://github.com/SAIR-Org/SAiR-MLOps-Blueprint)**
* **[SAiRCAMP](https://github.com/SAIR-Org/SAiRCAMP_1)**

MaaS-YT is specifically the **companion space for the personal YouTube channel** — where the focus is on taking on technical problems and working through them publicly.

---

# 🎬 Start Here

### Current Series

**[MLOps from First Principles](https://youtube.com/playlist?list=PLVM9Nqm8zLE0)**

Start with the production ML system.

### Next Challenge

**Head First into Inference Engineering**

Go underneath modern LLM inference.

### Building the Foundation

**Python Mastery Hub**

Develop the Python depth required for serious AI engineering.

---

> **We don't just learn the tools.**
>
> **We take on the problem, go underneath the abstraction, and figure out how it actually works.**

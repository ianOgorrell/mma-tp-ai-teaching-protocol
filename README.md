# MMA-TP — Modular Multi-State AI Teaching Protocol

**Published LLM tutoring protocol using JSON state specifications, gated interactions, and structured prompt/specification pairing.**

MMA-TP is a protocol-level framework for structuring multi-turn LLM tutoring interactions. It pairs an engineered runtime prompt with a structured JSON specification that defines interaction states, transitions, checkpoints, diagnostic signals, and response constraints.

The goal is not to modify the model or claim perfect deterministic control. The goal is to make LLM tutoring behavior more stable, structured, reusable, and teachable across longer instructional sessions.

The end result is a portable, copy/paste-ready tutor package that can follow a controlled curriculum while still allowing the model to answer questions, personalize explanations, and adapt to learner needs within defined boundaries.

MMA-TP is designed to be model-agnostic across capable transformer-based LLMs. Because the protocol lives in the interaction context rather than in model weights or platform-specific code, it can scale with improvements in model capability and context-window size. Larger context windows allow richer state specifications, longer lesson histories, more detailed diagnostic tracking, and more complete remediation logic.

Unlike a single natural-language prompt, MMA-TP gives the model a persistent structured scaffold for tracking where the learner is, what phase the tutor is in, which actions are allowed, and what kind of help should be provided at each step, and what should come next. This allows MMA-TP to efficiently "navigate" the context window as token count increases, where regular prompting becomes exponentially prone to a noisy self-attention mechanism, resulting in drift / hallucination.

---

## Publication 

**Title:** Modular Multi-State AI Teaching Protocol (MMA-TP)  
**Authors:** Ian Gorrell and Ethan Jordan  
**Corresponding author:** Ian Gorrell  
**Venue:** Proceedings of CONF-SPML 2026 Symposium: The Artificial Intelligence Tools & Applications  
**DOI:** https://doi.org/10.54254/2755-2721/2026.CH32181

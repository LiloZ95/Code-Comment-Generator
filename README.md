# 🧠 Code Comment Generator *(bonus)*
**24-Hour ML Challenge Submission**  
**Author:** Khalil Kurdi

---

## 💡 Overview

This project builds an intelligent **code comment generator** using pre-trained language models to help developers quickly understand what a given Python function does — **without requiring any manual documentation**.

We explored two models:

- 🦙 **CodeLlama 7B Instruct**: A powerful LLM fine-tuned for code instructions and summarization.
- 🧠 **Phi-1 (Microsoft)**: A lightweight, CPU-friendly model trained for logical and code-focused tasks.

> ⚠️ **Note:** I attempted fine-tuning on CodeT5 and Phi-based models using both LoRA and bitsandbytes techniques, but **the tuning degraded output quality**, producing repetitive or nonsensical completions. We therefore proceeded with **zero-shot inference** using the best available pre-trained checkpoints.

---

## 🧪 Model Details

### 🦙 CodeLlama-7B-Instruct
- Context-aware and instruction-tuned for summarizing or commenting code blocks
- Integrated using Hugging Face Transformers with 4-bit quantization for lower memory usage
- Best for **high-quality, natural language explanations**

### 🧠 Phi-1 (Microsoft)
- Lightweight LLM designed for reasoning and code synthesis
- Runs well on **CPU** and ideal for real-time VS Code-like extensions
- Best for **minimal compute environments**

---

## 🧭 Project Features

- Paste any **Python function** into the input box
- Choose your model: `CodeLlama` or `Phi-1`
- Receive a **summarized natural-language comment** describing the function's behavior
- Powered by Gradio for interactive testing

---


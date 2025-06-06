# KD_llama_1B-Knowledge-Distillation-for-LLaMA-3.2-1B
This project demonstrates knowledge distillation from LLaMA-3.2-3B-Instruct (teacher) to LLaMA-3.2-1B-Instruct (student). The goal is to transfer knowledge from a larger model into a smaller one to improve efficiency while maintaining performance.


🔧 Features
Loads teacher and student LLaMA models using Hugging Face Transformers.

Runs a simple prompt test to compare outputs.

Trains the student model using soft labels (logits) from the teacher model.

Uses wikitext-2-raw-v1 as training corpus.

Optimizes with KL divergence or MSE loss for token-level alignment.

📦 Installation
pip install transformers accelerate torch datasets

🚀 Quick Start
Run the notebook:
jupyter notebook KD_llama_1B.ipynb

📚 Dataset
WikiText-2 (raw) — used to generate prompts and soft labels.

📌 Notes
This is a lightweight example of offline distillation for causal language models.

Intended for small-scale experiments or educational use.

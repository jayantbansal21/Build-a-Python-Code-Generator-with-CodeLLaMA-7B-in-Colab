# Building-a-Python-Code-Generator-with-CodeLLaMA-7B-in-Colab

# Python Code Generator with Fine-Tuned CodeLLaMA 7B
Fine-tuned CodeLLaMA 7B in Google Colab (free tier) to generate Python code from natural language prompts. Deployed a Gradio UI for interactive demos.
Here's the link - https://colab.research.google.com/drive/1v16m_AEcJqGlWQJIIdU2MvAeAAwLaPvB?usp=sharing

## Features
- Fine-tuned on 5,000 CodeSearchNet examples.
- Optimized with 4-bit quantization and LoRA for Colab’s ~12GB RAM and T4 GPU.
- Generates Python functions (e.g., "Write a function to reverse a string" → `def reverse_string(s): return s[::-1]`).

## Setup
1. Open in Colab.
2. Run cells sequentially.
3. Access the Gradio UI via the public link.

## Challenges Overcome
- RAM crashes: Used quantization and bfloat16.
- Tokenizer padding: Set `eos_token` as pad token.
- Training setup: Added labels for loss computation.

Output screenshot - 
![Screenshot 2025-03-06 203754](https://github.com/user-attachments/assets/1ca468ed-28b4-4c50-aa6c-e574fcd7597a)

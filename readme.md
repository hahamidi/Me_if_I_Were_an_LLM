# Me_if_I_Were_an_LLM

This project distills my personal data (from my CV) into a **Large Language Model** using **PEFT** fine-tuning.  
The result is a lightweight **Qwen2.5-3B-Instruct** model that answers questions in my own “voice,” grounded entirely in my real experiences, skills, and achievements.

## Features
- Extracts text from a PDF CV.
- Generates instruction–completion pairs using OpenAI API.
- Fine-tunes Qwen model with LoRA for efficient, low-resource training.
- Interactive UI for asking questions as if you’re chatting with me.
- Fully offline after training—no external API calls during inference.

## Quick Start
1. Clone repo & install dependencies:
```bash
   pip install -r requirements.txt
````

2. Set your OpenAI API key:

```bash
   export OPENAI_API_KEY="sk-..."
```
3. Place your CV PDF in the repo and update `PDF_PATH` in the script.
4. Run the notebook or script to:

   * Generate dataset
   * Fine-tune model
   * Interactively query it

## Output Example

```
User: What is your PhD research focus?
Model: My research focuses on [your real answer from CV].
```




# 🧠 LLaMA 3.1–8B Fine-Tuned on Conspiracy QA — Using Unsloth + LoRA

This project fine-tunes Meta’s **LLaMA 3.1–8B Instruct** model on a **custom-built dataset** of over 430 conspiracy-themed question-answer pairs using [Unsloth](https://github.com/unslothai/unsloth) and **LoRA** for efficient training on a single GPU.

---

## 📌 Overview

The model was trained to generate answers on a wide range of conspiracy topics such as:

- Government secrecy  
- Alien coverups  
- Mind control programs  
- Historical manipulation  
- Secret organizations like Illuminati, Freemasons, etc.

The goal was to simulate a highly specific style of conversational generation that reflects internet conspiracy discussions — useful for both satire and serious exploration of belief modeling in LLMs.

---

## 🧪 Training Details

| Component              | Value                                |
|------------------------|--------------------------------------|
| Model Base             | `meta-llama/Llama-3.1-8B-Instruct`   |
| Frameworks Used        | 🤗 Transformers, 🧵 Unsloth, LoRA     |
| Dataset Size           | 431 examples                         |
| Parameters Trained     | 19.6M / 8B (0.25%)                   |
| Epochs                 | 4                                    |
| Batch Size             | 8 (2× per device × 4 grad accum)     |
| Fine-Tuning Time       | ~24 minutes in Colab T4              |

---

## 📂 Files in this Repo

- `Finetuning_Llama.ipynb` — Main notebook used for LoRA fine-tuning via Unsloth  
- `conspiracy_qa_data.json` — Final version of the dataset used for training  
- 🛠 **Data generation code not included**: It was iteratively modified and improved over time, making it unfit for static upload. However, the structure is easily reproducible from the JSON format.

---

## 🤖 Model Download

The merged and ready-for-inference model is hosted on Hugging Face:

🔗 **[haider-cheema28/llama3-conspiracy-model](https://huggingface.co/haider-cheema28/llama3-conspiracy-model)**

---


## 🧠 Author

**Haider Aitezaz Ali**  
AI enthusiast & student at NUST 🇵🇰  
📫 Let's connect on [LinkedIn](https://www.linkedin.com/in/haidercheema)

---


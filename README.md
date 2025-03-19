# 🌊🌊 SWELLS - A Specialized Workbench for the Explicit Learning of Linguistic Structures
[![Paper](http://img.shields.io/badge/Arxiv:2503.09454-B31B1B.svg)](https://arxiv.org/abs/2503.09454)

🚧 **Work in Progress!** This repository is an **early version** of SWELLS.

<p align="center">
  <picture>
    <!-- Dark Mode SVG -->
    <source srcset="SWELLS_dark.svg" media="(prefers-color-scheme: dark)">
    <!-- Light Mode SVG (Default) -->
    <img src="SWELLS.svg" alt="Synoptic Illustration" width="800">
  </picture>
</p>


SWELLS is a framework specially designed to study **explicit learning in Large Language Models (LLMs)** by means of machine translation experiments involving **constructed languages (conlangs)**. The dataset and scripts provided enable a controlled assessment of an LLM’s ability to learn and apply metalinguistic rules presented in grammar books.

## 🗂 **Project Overview**

This repository accompanies the research paper:

> **Explicit Learning and the LLM in Machine Translation**  
> *Malik Marmonier, Rachel Bawden, Benoît Sagot*  
> [Preprint available on ArXiv](https://arxiv.org/abs/2503.09454)

The project explores whether **LLMs can explicitly learn to generate specific linguistic phenomena** when provided with **relevant metalinguistic explanations from grammar book excerpts and dictionary entries**. It employs **cryptographically generated conlangs** as test environments to **control for prior knowledge interference and enhance result interpretability**.

## 🧩 **Usage**

This repository comprises a password-protected dataset (the password is `SWELLS`) located in the **[Releases section](https://github.com/mmarmonier/SWELLS/releases)**, as well as the following Jupyter notebooks, **which can be opened and run in Google Colab**, needed to interact with this complex set of files and perform the following tasks:

### **🔹 Training Data Generation**
To generate a **custom training set**, use the `1_SWELLS_Training_Set_Generator.ipynb` notebook. 

<a target="_blank" href="https://colab.research.google.com/github/mmarmonier/SWELLS/blob/main/1_SWELLS_Training_Set_Generator.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>
</a>

### **🔹 Supervised Fine-tuning**
To perform **supervised fine-tuning** on GPT-4o-mini, use the `2_SWELLS_Supervised_finetuner.ipynb` notebook.

<a target="_blank" href="https://colab.research.google.com/github/mmarmonier/SWELLS/blob/main/2_SWELLS_Supervised_finetuner.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>
</a>


### **🔹 Test Set Inference**
To perform **inference** on the test set using the OpenAI Batch API, use the `3_SWELLS_Test_Set_Inferencer.ipynb` notebook.

<a target="_blank" href="https://colab.research.google.com/github/mmarmonier/SWELLS/blob/main/3_SWELLS_Test_Set_Inferencer.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>
</a>


### **🔹 Evaluation**
To retrieve and **evaluate** inferences from OpenAI's batch API, use the `4_SWELLS_Evaluator.ipynb` notebook.

<a target="_blank" href="https://colab.research.google.com/github/mmarmonier/SWELLS/blob/main/4_SWELLS_Evaluator.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>
</a>


### 🔍 **For documentary purposes** 
We also provide an overview of our grammar template script (`grammar_template.ipynb` <a target="_blank" href="https://colab.research.google.com/github/mmarmonier/SWELLS/blob/main/Grammar_Template_Generator.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a> ).

🚨 **WARNING:** Some of these notebooks require an OpenAI API key, and users may incur significant costs upon running them. Be sure to check API pricing before proceeding.

## ⚖ **License**
This repository follows a **dual licensing model**:

- **Code** (scripts, notebooks) is released under the **[MIT License](https://opensource.org/license/mit/)**, allowing for open use, modification, and distribution with attribution.
- **Dataset** (training/dev/test sets) is licensed under **[CC BY-SA 4.0](http://creativecommons.org/licenses/by/4.0/)**, permitting sharing and adaptation with proper credit and under the same license terms.

## 📝 **Citation**
```
@misc{marmonier2025explicitlearningllmmachine,
      title={Explicit Learning and the LLM in Machine Translation}, 
      author={Malik Marmonier and Rachel Bawden and Benoît Sagot},
      year={2025},
      eprint={2503.09454},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2503.09454}, 
}
```

# Extending AskQE with Mistral-7B for Cross-Lingual QA Evaluation

This repository contains the report for the project **“Extending AskQE with Mistral-7B for Entailment-Aware Cross-Lingual QA Evaluation”**, developed at Politecnico di Torino.

The work extends the **AskQE** framework by integrating **Mistral-7B** as a question answering model to evaluate translation quality at the **answer level**, rather than relying on surface-level sentence similarity.

---

## 📄 Project Summary

The goal of this project is to assess whether translations preserve the **semantic meaning** of the source text. Instead of directly comparing sentences, the framework:
- Generates structured questions from the source text
- Extracts answers from the source, translations, and perturbed variants
- Compares answers using semantic, lexical, and logical metrics

This formulation allows translation evaluation to be treated as a **semantic entailment task**.

---

## 🧠 Main Contributions

- **Integration of Mistral-7B** into AskQE and comparison with LLaMA-8B  
- Evaluation under **monolingual, backtranslation, and direct cross-lingual** settings  
- Analysis of **critical vs minor translation perturbations**  
- Use of **SBERT, ROUGE, F1, and NLI (DeBERTa-v3)** for answer-level evaluation

---

## 📊 Key Findings

- Mistral-7B shows strong semantic alignment with LLaMA-8B at lower computational cost  
- Backtranslation is more semantically stable than direct cross-lingual QA  
- Critical perturbations significantly increase semantic inconsistency  
- Cross-lingual reasoning amplifies the impact of translation errors

---

## 🔗 References & Code

- Original AskQE: https://github.com/dayeonki/askqe

## 👥 Authors

Alessandro Ciarrocchi · Arianna Lezzi · Samuel Barbosa Gonçalves · Andrea Lanzillotta

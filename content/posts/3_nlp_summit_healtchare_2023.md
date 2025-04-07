---
date: 2023-04-07T22:18:37+01:00
title: "NLP Summit Healthcare 2023"
authors: ["diogo carapito"]
tags: ["NLP", "healthcare", "conference", "John Snow Labs"]
cover:
    image: 3_NLP-Summit-Healthcare-logo.png
    alt: NLP Summit Healthcare 2023
draft: false
---

This week I attended the **[NLP Summit Healthcare 2023](https://www.nlpsummit.org/)**, a free virtual event organized by the [John Snow Labs](https://www.johnsnowlabs.com/).
It was a great event with a lot of interesting talks. I’ll share some of my key takeaways.


## 1. Best practices when developing NLP models

Presented in the opening keynote by Dr. David Gondek, Chief Data Scientist at John Snow Labs, he sumarized some best practices that i found interesting as I’m beginning my NLP journey:
- **Test your models!** - why would you expect untested software to work? Test your models with real data and real use cases and assess it’s performance.
- **Don’t reuse academic models in production** - published research ≠ building reliable systems, testing and fine-tuning are essencial parts of developing a functional tool.
- **Test beyond accuracy** - Test for Robustness, Bias, Fairness, Toxicity, Efficiency, Safety. John Snow Labs developed **[NLP test](https://nlptest.org/)** to help with model testing beyond regular benchmarks.

## 2. Mitigating bias in healthcare language models

Gaurav Kaushik from ScienceIO presented a talk about **mitigating bias** in **healthcare language models** and the importance of its evaluation. **Performance benchmarks** lack the statistical power, they aren’t well validated enough and **don’t incentivize the use of biased systems**.

- **Algorithmic bias** 
  - Systematic and repeatable errors that yield unfair outcomes which benefit certain groups over others 
  - Healthcare LP systems will influence clinical outcomes and therefore will mitigate or exacerbate outcome disparities 
- **Selection Bias** - data used in training the model does not represent real-world
- **Label bias** - mismatch between annotations and target, _e.g._ due to judgement, human error, or label ambiguity
- **Training bias** - models amplify biases in the training data
- **Semantic bias** - bias from input representations such as inappropriate word associations
- **Demographic bias** - improper sensitivity to race or gender, or impaired performance on attributes related to subgroups
- **Domain Bias** - error bias in medical subdomains, such as disease areas, which can impair generalization

Check this article for further information: [Beyond Accuracy: Behavioral Testing of NLP Models with CheckList](https://aclanthology.org/2020.acl-main.442.pdf)
## 3. Prototypical Networks for Interpretable Diagnosis Prediction

**Betty van Aken** from **DATEXIS Research Group** presented a language model that **makes predictions** based on parts of the text that are **similar to prototypical patients** providing justifications that doctors understand.
It uses a prototypical network with label-wise attention to **find the most similar patients to the input text** and then uses a transformer to **predict the diagnosis**.
This is a great example of how NLP can be used in healthcare space and opens the door to a lot of interesting applications.

Check their [demo](https://protopatient.demo.datexis.com/) and the paper here: [This Patient Looks Like That Patient: Prototypical Networks for Interpretable Diagnosis Prediction from Clinical Text](https://aclanthology.org/2022.aacl-main.14.pdf)
## 4. EHR-Safe: Generating High-Fidelity and Privacy-Preserving Synthetic Electronic Health Records

AI in healthcare has important **privacy concerns**, especially when dealing with **sensitive data like Electronic Health Records** (EHR). Cloud AI Team suggested that one way to overcome this challenge is to generate high-fidelity, privacy-preserving synthetic EHR data.
They proposed a generative modeling framework, EHR-Safe, that **can generate highly realistic synthetic EHR data** that are robust against privacy attacks.

Check their paper here: [EHR-Safe: Generating high-fidelity and privacy-preserving synthetic electronic health records](https://ai.googleblog.com/2022/12/ehr-safe-generating-high-fidelity-and.html)

## 5. Some organizations that are doing interesting work in NLP in healthcare:

- **[John Snow Labs](https://www.johnsnowlabs.com/)** - organizer of the summit and creator of state-of-the-art NLP in healthcare, like [NLP test](https://github.com/johnsnowlabs/nlptest) and [SparkNLP](https://sparknlp.org/)
- **[Discovery Lab](https://discoverylab.ai/)** - Lab funded by Elsevier, Vrije Universiteit Amsterdam and the University of Amsterdam that operates at the crossroads of Knowledge Representation, Machine Learning and Natural Language Processing.
- **[NeuralMed](https://www.neuralmed.ai/en)** - a healthcare AI company that develops AI solutions for the healthcare industry.
- **[Science IO](https://www.science.io/)** - transforms medical text into enriched data to build solutions that improve patient care.
- **[DATEXIS](https://github.com/DATEXIS)** - Data Science and Text-based Information Systems (DATEXIS) group at Beuth University of Applied Sciences Berlin

---

This is a list of some interesting projects that were presented at the summit:

- **[Spark NLP](https://sparknlp.org/)** - an open source text processing library for Python, Java, and Scala.
- **[NLP test](https://nlptest.org/)** - a suit of tests to help mitigate bias for NLP models.
- **[BioMedLM](https://huggingface.co/stanford-crfm/BioMedLM)** - a GPT style language model trained on biomedical abstracts and papers.
- **[BioGPT](https://huggingface.co/microsoft/biogpt)** - a pre-trained language models on the biomedical domain.
- **[ProtoPatient](https://protopatient.demo.datexis.com/)** Demo - diagnostic predictions using clinical text and prototypical patients.
- **[Clinical IE](https://huggingface.co/datasets/mitclinicalml/clinical-ie)** - a Large Language Model for information extraction of Clinical Text

---

Finally, I’ll share some of the **articles** that were cited in the talks:

- [Dataset Carto graphy: Mapping and Diagnosing Datasets with Training Dynamics](https://arxiv.org/abs/2009.10795)
- [Five sources of bias in natural language processing](https://compass.onlinelibrary.wiley.com/doi/10.1111/lnc3.12432)
- [Beyond Accuracy: Behavioral Testing of NLP Models with CheckList](https://aclanthology.org/2020.acl-main.442.pdf)
- [Quantifying Social Biases in NLP: A Generalization and Empirical Comparison of Extrinsic Fairness Metrics](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00425/108201/Quantifying-Social-Biases-in-NLP-A-Generalization)
- [TruthfulQA: Measuring How Models Mimic Human Falsehoods](https://arxiv.org/pdf/2109.07958.pdf)
- [This Patient Looks Like That Patient: Prototypical Networks for Interpretable Diagnosis Prediction from Clinical Text](https://aclanthology.org/2022.aacl-main.14.pdf)
- [Physician Global Assessment (PGA)](https://assesschild.com/physician-global-assessment)
- [EHR-Safe: Generating High-Fidelity and Privacy-Preserving Synthetic Electronic Health Records](https://www.researchsquare.com/article/rs-2347130/v1)
- [Open AI Fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning)


---

There were many more interesting sessions I didn’t describe here, visit [https://www.nlpsummit.org/](https://www.nlpsummit.org/) if you want further information.
I’ll be there next year for sure!
Thanks for reading!

P.S. Copilot helped writing this blog post.
LLMs are amazing and I’m excited to see what the future holds for NLP!

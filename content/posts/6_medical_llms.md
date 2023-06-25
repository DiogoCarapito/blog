---
title: "Medical Large Language Models"
date: 2023-06-25T09:10:00+01:00
authors: ["diogo carapito"]
tags: ["conference", "LLM", "healthcare", "John Snow Labs"]
draft: false
cover:
    image: 6_Medical Large Language Models for Clinical Text Summarization Information Extraction and Question Answering.png
    alt: LLM_Bootcamp_2023
---

I attended last week the **Medical Large Language Models for Clinical Text Summarization, Information Extraction, and Question Answering** from [John Snow Labs](https://www.johnsnowlabs.com/).
I'm sharing my notes here.

# LLMs

LLMs and NLP in general have are providing new tools to solve existing problems in healthcare.
Where is a list of some new tools that are available today:
- Question Answering
- Text Summarization
- Text Generation
- Information extraction (from clinical notes)
- Relation extraction (symptoms related to a disease)
- Entity recognition (like ICD-10 code extraction)
- Chatbots

Many open source LLMs available today have close performance to the best commercial state-of-the-art models, like GPT-4, GPT-3.5-turbo form OpenAI or Claude from [Anthropic](https://www.anthropic.com/index/introducing-claude).
The last tend to be general purpose, powerful, but extremely expensive to train.
The open source models tend to lack performance in a broad sense but can be fine-tuned to specific tasks.
This field is moving fast, witch means that there is much potential for innovation, but also it's a challenge to keep up with the state-of-the-art.

Here is an overview of **tasks** that **Medical LLMs** can perform today: 

# LLMs in Healthcare

### 1. Close book Q&A:

Question answering using [BioGPT JSL](https://nlp.johnsnowlabs.com/2023/04/18/biogpt_chat_jsl_conversational_en.html) as the base model and a knowledge base.

*demo available here: https://demo.johnsnowlabs.com/healthcare/MEDICAL_LLM/*

### 2. Medical text generation

The same can also generate text, like an elaborate response from more open question,
creating synthetic text or synthetic patients.
![test](/post_images/6_text_generation.png)
*Demo available here: https://demo.johnsnowlabs.com/healthcare/MEDICAL_LLM/*

*(nice implementation with [streamlit](https://streamlit.io/) btw)*

### 3. Clinical text Summarization

One of the **most popular** uses of LLMs in medical field is **clinical summarization**.
An obvious use case is to summarize a **patient's medical history**, since it can get very long and have repeated information
This summarization has its own specificities, like the need to **preserve the medical terminology** and the need to **preserve the order of the events**.

*demo available here: https://demo.johnsnowlabs.com/healthcare/MEDICAL_LLM/*

### 4. Biomedical Research text Summarization

A tool to help to deal with the avalanche of new research papers that are being published.
It makes it easier to automate the process of reading and summarizing the papers. 

### 5. Patient Question text Summarization 

A way to resume the patient's question to the doctor, so that the doctor can quickly understand the patient's concern.

![patient question text](/post_images/6_patient_questions.png)



# No-Code Medical Chatbots

Another interesting concept is **no-code implementations** that JNL are developing,
available at https://www.johnsnowlabs.com/nlp-lab/.

It can used to create **natural language interfaces** to query databases, both clinical records and biomedical research.

![query search](/post_images/6_query_serch.png)

This seems very interesting to apply in a **Business Intelligence** + **healthcare** context.
The user could help accelarate and make more widespread the adoption of BI practices in the field.



It was also proposed 3 key requirements for chatbots to be **compliant with regulation** (like new legislation that is being currently discussed in EU parliament)
- **No Data Sharing**: Clinical data is sensitive. No data is shared through cloud, APIs and 3rd parties. Secure solutions under the firewall
- **No _BS_**: no hallucinations or unexplained results. Every answer can be explained and backed by a reference
- **No Test Gaps**: test for robustness, fairness, and bias, data leackege or toxicity. Able to prove to customers and regulators

---

I'm **amazed** and **overwhelmed** by the potential of LLMs in the medical field. The possibilities are limitless.

The vod of the webcast can be found here: https://www.carahsoft.com/learn/event/45747-medical-large-language-models-for-clinical-text-summarization-information-extraction-and-question-answering


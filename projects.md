---
layout: page
title: Projects
permalink: /projects/
---

# My Projects

Every project I take on starts with a simple question: _“What problem am I really solving?”_ Below are some of my
favorite projects, explained through the challenges they addressed, the routes I took, and the impact they delivered.

## 🧾 RAG-Based Chatbot for Life Insurance Policy Understanding

[View on GitHub](#)

Insurance policies are notoriously difficult to read — full of jargon, dense tables, and scattered clauses. I wanted to
make this process human-friendly.

**The Route I Took:**

-   Extracted text and tables from policy PDFs using **pdfplumber**.
-   Broke them into **500-token chunks with 50-token overlap** for better contextual retrieval.
-   Stored embeddings with **OpenAI ada-002** vectors inside **ChromaDB**.
-   Designed a **dual-stage retrieval system**: first vector similarity, then a **CrossEncoder MiniLM** reranker for
    accuracy.
-   Finally, passed refined results into **GPT-3.5 Turbo**, with hallucination controls to ensure answers stayed
    grounded.

**The Result:** A chatbot that can answer real-world queries like _“Can I surrender this policy?”_ or _“How is the claim
processed?”_ with clarity and accuracy. It transformed frustrating policy documents into an interactive Q&A tool —
making insurance more accessible.

## 🚲 Bike Demand Prediction

[View on GitHub](#)

For companies like Boom Bikes, the challenge is not just selling bikes — it’s predicting **how many will be rented
tomorrow**. Overstocking is wasteful, understocking is bad business.

**The Route I Took:**

-   Collected weather, seasonal, and user data.
-   Used **Scikit-learn** with a **Multiple Linear Regression (MLR)** model.
-   Applied **VIF-based feature pruning** and scaling to remove multicollinearity.

**The Result:** An R² score of **0.82** — strong predictive power. This meant automated inventory management became
feasible, helping optimize fleet availability and reducing lost revenue.

## 🩺 Skin Cancer Detection with CNN

[View on GitHub](#)

Dermatologists face the challenge of distinguishing between multiple skin cancer subtypes early on — where accurate
detection matters most.

**The Route I Took:**

-   Built a **TensorFlow + Keras** CNN pipeline.
-   Applied **rotation and scaling augmentations** to enrich training data.
-   Added dropout layers to reduce overfitting.

**The Result:** Achieved **92% test accuracy** across **7 skin cancer subtypes**. This project demonstrated how AI could
support doctors in early diagnosis, potentially saving lives.

## ✋ Gesture Recognition with 3D-CNN

[View on GitHub](#)

Human-computer interaction is evolving — and I wanted to explore how machines could _see and understand gestures_.

**The Route I Took:**

-   Designed a **Conv3D + ConvLSTM spatiotemporal model**.
-   Tuned hyperparameters like learning rate and batch size.
-   Regularized with **L2 penalties** to stabilize training.

**The Result:** Achieved **78% validation accuracy** on a challenging video dataset. The project laid the foundation for
gesture-controlled interfaces in AR/VR environments.

## 🌬️ Cylindrical Filter Simulator – Air Filtration System Modeling Tool

[View on GitHub](#)

Industrial filters are everywhere — but optimizing them is still largely trial and error. I wanted to bring **science +
AI** into filtration design.

**The Route I Took:**

-   Built a **multi-physics simulator** in Python.
-   Modeled airflow, pressure drop, dust loading, and efficiency.
-   Added **geometry optimization** features and a real-world media database.
-   Exported publication-ready plots (Matplotlib), reports (ReportLab PDF), and datasets (JSON/CSV).

**The Result:** A research-grade tool with **Colab UI integration**, making it accessible to scientists and engineers.
It showcased how AI-powered design tools can accelerate innovation in manufacturing.

## ✈️ Travel Experience Chatbot (Ongoing)

[View on GitHub](#)

Planning a trip means juggling multiple apps: flights, hotels, weather, itineraries. I asked: _“What if one AI could do
it all?”_

**The Route I Took:**

-   Engineered a **Flask-based chatbot**.
-   Integrated **OpenAI GPT**, **Amadeus API**, and weather APIs.
-   Applied prompt engineering for **personalized itineraries**.

**The Result (so far):** A single interface that gives users real-time, customized travel plans — a project I’m still
refining, but one that excites me for its everyday usefulness.

## 📰 Semantic Fake News Detection

[View on GitHub](#)

The spread of fake news is a global challenge. I wanted to see if semantics — the _meaning_ of words — could help
machines separate fact from fiction.

**The Route I Took:**

-   Preprocessed text with **lemmatization + POS tagging**.
-   Generated embeddings using **Word2Vec**.
-   Trained classifiers: Logistic Regression, Random Forest, and Decision Tree.

**The Result:** The **Logistic Regression pipeline** reached **91% accuracy and 0.906 F1 score**. The project proved how
**simple yet semantic-rich models** can fight misinformation effectively.

✨ Each of these projects started as curiosity but ended up becoming solutions that others could use, learn from, or
build upon. My hope is that they inspire you to imagine your own — because every project starts with a single _“what
if?”_.

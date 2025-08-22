---
layout: page
title: My Projects
permalink: /projects/
---

<br>Every project I take on starts with a simple question: _“What problem am I really solving?”_ Below are some of my
favorite projects, explained through the challenges they addressed, the routes I took, and the impact they delivered.

<hr class="neon-line">

## 🧾 RAG-Based Chatbot for Life Insurance Policy Understanding
<div style="text-align: center;">
<a href="https://github.com/AnishRane-cox/Insurance-HelpMateAI.git" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>Insurance policies are notoriously difficult to read and are full of jargon, dense tables, and scattered clauses. I
wanted to make this process human-friendly.

<br>**The Route I Took:**

-   Extracted text and tables from policy PDFs using **pdfplumber**.
-   Broke them into **500-token chunks with 50-token overlap** for better contextual retrieval.
-   Stored embeddings with **OpenAI ada-002** vectors inside **ChromaDB**.
-   Designed a **dual-stage retrieval system**: first vector similarity, then a **CrossEncoder MiniLM** reranker for
    accuracy.
-   Finally, passed refined results into **GPT-3.5 Turbo**, with hallucination controls to ensure answers stayed
    grounded.

<br>**The Result:** A chatbot that can answer real-world queries like _“Can I surrender this policy?”_ or _“How is the
claim processed?”_ with clarity and accuracy. It transformed frustrating policy documents into an interactive Q&A tool
making insurance more accessible.

<hr class="neon-line">

## 🚲 Bike Demand Prediction
<div style="text-align: center;">
<a href="https://github.com/AnishRane-cox/Bike-Demand-Prediction-MLR.git" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>For companies like Boom Bikes, the challenge is not just selling bikes it’s predicting **how many will be rented
tomorrow**. Overstocking is wasteful, understocking is bad business.

<br>**The Route I Took:**

-   Collected weather, seasonal, and user data.
-   Used **Scikit-learn** with a **Multiple Linear Regression (MLR)** model.
-   Applied **VIF-based feature pruning** and scaling to remove multicollinearity.

<br>**The Result:** An R² score of **0.82** strong predictive power. This meant automated inventory management became
feasible, helping optimize fleet availability and reducing lost revenue.

<hr class="neon-line">

## 🩺 Skin Cancer Detection with CNN
<div style="text-align: center;">
<a href="https://github.com/AnishRane-cox/Skin-Cancer-Detection-using-CNN.git" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>Dermatologists face the challenge of distinguishing between multiple skin cancer subtypes early on where accurate
detection matters most.

<br>**The Route I Took:**

-   Built a **TensorFlow + Keras** CNN pipeline.
-   Applied **rotation and scaling augmentations** to enrich training data.
-   Added dropout layers to reduce overfitting.

<br>**The Result:** Achieved **92% test accuracy** across **7 skin cancer subtypes**. This project demonstrated how AI
could support doctors in early diagnosis, potentially saving lives.

<hr class="neon-line">

## ✋ Gesture Recognition with 3D-CNN
<div style="text-align: center;">
<a href="https://github.com/AnishRane-cox/Gesture-Recognition-using-3D-CNN.git" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>Human-computer interaction is evolving and I wanted to explore how machines could _see and understand gestures_.

<br>**The Route I Took:**

-   Designed a **Conv3D + ConvLSTM spatiotemporal model**.
-   Tuned hyperparameters like learning rate and batch size.
-   Regularized with **L2 penalties** to stabilize training.

<br>**The Result:** Achieved **78% validation accuracy** on a challenging video dataset. The project laid the foundation
for gesture-controlled interfaces in AR/VR environments.

<hr class="neon-line">

## 🌬️ Cylindrical Filter Simulator – Air Filtration System Modeling Tool
<div style="text-align: center;">
<a href="https://github.com/AnishRane-cox/Cylindrical-Filter-Simulator.git" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>Industrial filters are everywhere — but optimizing them is still largely trial and error. I wanted to bring
**science + AI** into filtration design.

<br>**The Route I Took:**

-   Built a **multi-physics simulator** in Python.
-   Modeled airflow, pressure drop, dust loading, and efficiency.
-   Added **geometry optimization** features and a real-world media database.
-   Exported publication-ready plots (Matplotlib), reports (ReportLab PDF), and datasets (JSON/CSV).

<br>**The Result:** A research-grade tool with **Colab UI integration**, making it accessible to scientists and
engineers. It showcased how AI-powered design tools can accelerate innovation in manufacturing.

<hr class="neon-line">

## ✈️ Travel Experience Chatbot (Ongoing)
<div style="text-align: center;">
<a href="#" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>Planning a trip means juggling multiple apps: flights, hotels, weather, itineraries. I asked: _“What if one AI could
do it all?”_

<br>**The Route I Took:**

-   Engineered a **Flask-based chatbot**.
-   Integrated **OpenAI GPT**, **Amadeus API**, and weather APIs.
-   Applied prompt engineering for **personalized itineraries**.

<br>**The Result (so far):** A single interface that gives users real-time, customized travel plans a project I’m still
refining, but one that excites me for its everyday usefulness.

<hr class="neon-line">

## 📰 Semantic Fake News Detection
<div style="text-align: center;">
<a href="https://github.com/AnishRane-cox/Semantic-Fake-News-Detector.git" class="cta-button" target="_blank" rel="noopener noreferrer">View on GitHub</a>
</div>
<br>The spread of fake news is a global challenge. I wanted to see if semantics the _meaning_ of words could help
machines separate fact from fiction.

<br>**The Route I Took:**

-   Preprocessed text with **lemmatization + POS tagging**.
-   Generated embeddings using **Word2Vec**.
-   Trained classifiers: Logistic Regression, Random Forest, and Decision Tree.

<br>**The Result:** The **Logistic Regression pipeline** reached **91% accuracy and 0.906 F1 score**. The project proved
how **simple yet semantic-rich models** can fight misinformation effectively.

<hr class="neon-line">

✨ Each of these projects started as curiosity but ended up becoming solutions that others could use, learn from, or
build upon. My hope is that they inspire you to imagine your own because every project starts with a single _“what
if?”_.

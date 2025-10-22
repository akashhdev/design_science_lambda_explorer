# Design Science – Lambda Sweeping

This repository contains the **interactive web demo** for the research project **“Design Science – Lambda Sweeping.”**  
The demo visualizes how an AI classification system can be tuned based on **user-defined error cost preferences**, expressed through the **λ (lambda) parameter**.

🔗 **Live Demo:** [https://main.d3ipp6oq5bamax.amplifyapp.com/](https://main.d3ipp6oq5bamax.amplifyapp.com/)  
Currently hosted on **AWS Amplify**.

---

## 🧠 Project Summary
Traditional AI models optimize **accuracy**, assuming all mistakes are equally bad.  
In real-world applications, different errors have **different consequences** — for example:

- **False Positive (FP):** Wrongly fines an innocent driver.  
- **False Negative (FN):** Misses an actual violator.  

To align AI behavior with these real-world preferences, this project introduces **λ (lambda)** as a control factor:

\[
λ = \frac{Cost_{FP}}{Cost_{FN}}
\]

- **High λ:** System avoids false positives (becomes more cautious).  
- **Low λ:** System avoids false negatives (becomes more aggressive).

This process of testing how performance changes across λ values is called **Lambda Sweeping**.

---

## 🌐 Demo Overview
The web demo (`index.html`) illustrates how adjusting λ and decision thresholds changes:
- **Precision** (accuracy of positive detections)
- **Recall** (coverage of true positives)
- **Overall cost** under different λ values

It is a **conceptual simulation**, not a live machine learning model.  
All calculations are performed in-browser to help visualize trade-offs interactively.

---

## ⚙️ Technologies Used
- **HTML**, **CSS**, **JavaScript**  
- Optional visualization library (e.g., Chart.js or D3.js)  
- Hosted on **AWS Amplify** for deployment and accessibility  
- No backend or external model dependencies  

---

## 🚀 How to Use
1. Visit the live demo:  
   🔗 [https://main.d3ipp6oq5bamax.amplifyapp.com/](https://main.d3ipp6oq5bamax.amplifyapp.com/)  
   *(or open `index.html` locally in your browser)*  
2. Adjust the **λ** and **threshold** sliders to observe changes in:  
   - Precision  
   - Recall  
   - Overall cost  

---

## 📚 Background
This demo is part of the **Design Science Research (DSR)** framework, emphasizing the *creation and evaluation of practical artifacts*.  
Rather than designing a new AI model, this project focuses on **decision-level optimization** — showing how existing models can be tuned to reflect ethical or operational priorities.

Example applications:
- **Traffic enforcement:** Minimize false fines (λ high).  
- **Medical diagnosis:** Minimize missed cases (λ low).

---

© 2025 National Chung Cheng University – For academic and educational use only.

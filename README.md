# Design Science – Lambda Sweeping (Interactive Demo)

## 📘 Overview
This repository contains the **interactive web demo** for the research project **“Design Science – Lambda Sweeping.”**  
The demo visualizes how an AI classification system can be tuned according to user-defined **error cost preferences**, represented by the **λ (lambda) parameter**.

The project follows the **Design Science Research (DSR)** methodology — focusing on building and evaluating a *preference-guided AI decision framework* rather than training a new model from scratch.

---

## 🧠 Concept Summary

### 🔹 The Problem
Traditional AI classifiers optimize **overall accuracy**, assuming all errors are equally costly.  
However, in real-world scenarios (like traffic enforcement or healthcare), different mistakes have **unequal consequences**.

Example:
- **False Positive (FP):** Wrongly fines an innocent driver.  
- **False Negative (FN):** Misses a real violation.  

Police departments prefer **fewer false positives**, even if it means missing some violations.

---

### 🔹 The Lambda Framework
The project introduces a **cost model**:

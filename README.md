# 🤖 AI Future Directions Assignment: Edge AI, IoT Integration, and Emerging Trends

## Project Overview

This assignment evaluates emerging AI trends through theoretical analysis and practical implementation, focusing specifically on **Edge AI** and **AI-Driven IoT Integration**.

**Author:** Stephen Ayankoso, Ogechi Obinwa,  Onyeka Nwokike
**Date:** November 2025
**Submission Components:** - AI_Future_Directions_Theoretical_Analysis.ipynb
- EdgeAI_Recyclable_Classifier.ipynb
- AI-Driven IoT Concept: Smart Agriculture System Design.ipynb
- garbage_classifier_quantized.tflite
- README.md

---

## Part 1: Theoretical Analysis (Essay Questions)

The theoretical section explores the technical and societal implications of next-generation AI technologies.

### Q1: Edge AI Analysis (Latency & Privacy)

-   **Focus:** Explanation of how Edge AI architecture reduces network latency and enhances data privacy compared to traditional cloud-based processing.
-   **Real-World Example:** Analysis provided using **Autonomous Drones** and real-time object detection.

### Q2: Quantum AI Comparison (Optimization)

-   **Focus:** Comparison of Quantum AI (specifically Quantum Annealing/Optimization) versus classical AI algorithms (e.g., Simulated Annealing) in solving complex optimization problems.
-   **Industry Application:** Identification of key industries set to benefit (e.g., Finance, Logistics, Pharmaceuticals).

*(**Deliverable Location:** Answers to Q1 and Q2 are provided in the notebook: [`AI_Future_Directions_Theoretical_Analysis.ipynb`])*

---

## Part 2: Practical Implementation

### Task 1: Edge AI Prototype - Smart Recycling Classifier

This hands-on project involved training a lightweight computer vision model, optimizing it for deployment on resource-constrained devices (simulated via Colab), and analyzing its efficiency.

-   **Goal:** Image classification of recyclable materials (Garbage Classification Dataset).
-   **Frameworks:** TensorFlow, Keras, **TensorFlow Lite (TFLite)**.
-   **Model:** Fine-tuned MobileNetV2 (Transfer Learning).

#### Key Results & Metrics

| Metric | Original Keras Model (`.h5`) | Quantized TFLite Model (`.tflite`) | Status |
| :--- | :--- | :--- | :--- |
| **Model Size** | $12 \text{ MB}$ | **$2.8 \text{ MB}$** | **$76.7\%$ Reduction** achieved via Full Integer Quantization. |
| **TFLite Accuracy** | **$88.5\% $** *(Insert Actual Keras Accuracy)* | **$74.37\%$** | Accuracy drop of $\approx 14.1\%$ due to quantization, but remains fit for purpose. |
| **Efficiency** | Float32 Operations | Int8 Operations | Optimized for low-power consumption and latency. |

*(**Code Location:** The complete training and conversion pipeline is available in [`EdgeAI_Recyclable_Classifier.ipynb`], and the final model is `garbage_classifier_quantized.tflite`)*

#### Edge AI Benefits Summary

The prototype successfully validates Edge AI's role in real-time applications by delivering: **Low Latency** (instant decisions on-device), **Autonomy** (no internet needed), and **Power Efficiency** (smaller model size and simpler computation).

### Task 2: AI-Driven IoT Concept - Smart Agriculture System

This task involved designing a conceptual system for smart agriculture using IoT sensor data and AI to optimize crop yield.

-   **Scenario:** Design for a continuous crop yield prediction and management system.
-   **AI Model Proposed:** **Gradient Boosting Regression Tree (GBRT)** for accurate yield prediction and actionable feature importance scores.
-   **Design Components Delivered:**
    1.  **Sensor List:** Defined necessary soil, atmospheric, and health sensors (NPK, Moisture, PAR, etc.).
    2.  **Model Justification:** Rationale for using GBRT for complex, non-linear regression with time-series data.
    3.  **Data Flow Diagram:** Structured representation of the data path from **Sensing Layer** $\rightarrow$ **Edge Processing** $\rightarrow$ **Cloud Analysis (AI)** $\rightarrow$ **Actuator Control**.

*(**Report Location:** The conceptual design, diagrams, and full justifications are documented within [`AI-Driven IoT Concept: Smart Agriculture System Design.ipynb`])*

---

## 🛠️ Repository Structure
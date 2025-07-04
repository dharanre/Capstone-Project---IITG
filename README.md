# Capstone-Project---IITG
Dynamic Urban Parking Pricing Engine Summer Analytics 2025 - Final Submission Report

# 🚗 Dynamic Urban Parking Pricing Engine

A real-time, data-driven pricing system for 14 urban parking lots using streaming data, economic principles, and machine learning models — built entirely using **Python, NumPy, Pandas, and Pathway**.

> 🧠 Developed as part of **Summer Analytics 2025**, hosted by the **Consulting & Analytics Club × Pathway**.

---

## 📌 Project Objective

Urban parking is limited and highly demanded. Static pricing causes either underutilization or overcrowding.  
This project aims to solve that using:

- Real-time dynamic pricing based on demand and competition
- Real-world features like traffic, queue, vehicle type, special events
- A multi-stage pricing model pipeline

---

## 🧰 Tech Stack

| Layer              | Tools Used                 |
|-------------------|----------------------------|
| Language           | Python (NumPy, Pandas)     |
| Real-time Engine   | Pathway                    |
| Visualization      | Bokeh                      |
| Environment        | Google Colab               |
| Repo Hosting       | GitHub                     |

---

## 🧱 Architecture Diagram

```mermaid
flowchart TD
  A[dataset.csv (historical + streaming data)] --> B[Pathway Stream Engine]
  B --> C[Feature Engineering<br>(occupancy, queue, traffic, etc)]
  C --> D{Pricing Models}
  D --> D1[Model 1:<br>Baseline Linear]
  D --> D2[Model 2:<br>Demand-Based]
  D --> D3[Model 3:<br>Competitive (optional)]
  D --> E[Pricing Output (per lot)]
  E --> F[Bokeh Visualizer (Real-time Plots)]

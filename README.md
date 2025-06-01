# Loan Application Analysis – BPI Challenge 2017

This project analyzes the BPI Challenge 2017 dataset using a combination of machine learning and Power BI. It focuses on identifying factors that influence loan application success and visualizing how applications are processed.

---

## Dataset

The [BPI Challenge 2017 dataset](https://data.4tu.nl/articles/dataset/BPI_Challenge_2017/12696884) contains event logs from a Dutch financial institution’s loan application system. Each record logs an event in a case, with attributes such as:

- `case`: Unique application ID
- `event`: Activity name (e.g., A_Create Application, A_Submitted)
- `LoanGoal`, `CreditScore`, `ApplicationType`, and timestamps

---

## Key Analyses

### 1. Feature Importance (Random Forest)

A random forest classifier was trained to predict application success (presence of the `A_Pending` event). The model identified the following as the most important features:
- Case duration
- Loan goal categories
- Credit score
- Submission method

---

### 2. Power BI Insights

The Power BI dashboard compares success vs. failure across:
- Loan goal
- Case duration (in days)
- Submission method (in person vs. not)

![Power BI Dashboard](https://github.com/user-attachments/assets/8763d1c8-54f9-43cd-9c02-08427856fd20)

---

### 3. Process Mining View

A process model shows the most frequent paths through the loan application lifecycle.

![Process Flow Diagram](https://github.com/user-attachments/assets/8a275d6f-583f-453a-bb43-0d8ae2d8200d)

---

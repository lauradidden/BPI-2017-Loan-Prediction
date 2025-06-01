# Loan Application Analysis – BPI Challenge 2017

This project analyzes the BPI Challenge 2017 dataset using a combination of machine learning and Power BI. It focuses on identifying factors that influence loan application success and visualizing how applications are processed.

---

## Power BI Visualization

The Power BI dashboard compares success vs. failure across:
- Loan goal
- Case duration (in days)
- Submission method (in person vs. not)

![Power BI Dashboard](https://github.com/user-attachments/assets/8763d1c8-54f9-43cd-9c02-08427856fd20)

---

## Feature Importance Analysis (Random Forest)

A random forest classifier was trained to predict application success (presence of the `A_Pending` event). The model identified the following as the most important features:
- Case duration
- Loan goal categories
- Credit score
- Submission method

---

## Process Model View

A process model shows the most frequent paths through the loan application lifecycle.

![Process Flow Diagram](https://github.com/user-attachments/assets/8a275d6f-583f-453a-bb43-0d8ae2d8200d)

---

## Dataset: BPI Challenge 2017

The BPI Challenge 2017 dataset contains event logs from a Dutch financial institution, capturing the full lifecycle of thousands of personal loan applications. Each row represents a single event in a case, such as application submission, offer creation, or cancellation.

Key attributes include:
- `case`: unique application ID  
- `event`: type of activity (e.g., A_Submitted, O_Created)   
- `time`: timestamp for process mining and duration analysis
- `Case Attributes` such as: `LoanGoal`, `CreditScore`, `RequestedAmount`, and `MonthlyCost` 

---

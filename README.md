# Student Spending & Expenses Behavior Analysis

A comprehensive Power BI dashboard project analyzing the spending habits, savings behavior, financial discipline, and financial risk levels of Indian college students.

Prepared by:
- Reshaan Nadar
- Devansh Kanungo
- Anish Nair

---

## Project Overview

This project explores how college students manage their monthly allowances, spending, and savings across different academic disciplines and years of study.

Using Power BI, Power Query, and DAX, the project transforms survey data into interactive dashboards that uncover financial patterns, risk groups, and actionable insights for improving student financial literacy.

The analysis is based on:
- 82 student respondents
- 10+ financial and demographic variables
- 3 interactive Power BI dashboard pages

---

## Objectives

This project aims to answer key financial behavior questions such as:

- What are the major spending categories for students?
- Which academic courses save the most?
- Does expense tracking improve savings?
- Which students fall into high financial risk categories?
- How do spending and savings vary by gender and academic year?

---

## Tools & Technologies Used

- Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Excel / CSV Dataset
- Data Visualization Techniques

---

## Dashboard Pages

### 1. Student Spending Behavior Analysis
Focus Areas:
- Total student spending
- Average allowance and expenses
- Spending trends over time
- Spending by course
- Payment method analysis
- Food expense comparison

Key Findings:
- Transport is the highest spending category
- M.B.B.S students spend the most
- 80.49% students use digital payments
- Students collectively spend ₹820K monthly

---

### 2. Student Saving Behavior Analysis
Focus Areas:
- Average savings
- Savings rate
- Savings by course
- Savings by gender
- Savings trend analysis
- Savings by year of study

Key Findings:
- B.Com students show the highest savings
- 4th year students save significantly more
- Female students save more on average
- Overall savings rate: 38.89%

---

### 3. Student Financial Behavior Analysis
Focus Areas:
- Risk level segmentation
- Expense tracking behavior
- Allowance vs spending comparison
- Financial discipline analysis
- Source of student income

Key Findings:
- Expense tracking strongly improves savings
- Moderate-risk students form the largest segment
- Over 80% of students rely on parental funding
- Tracking frequency directly correlates with savings growth

---

## Dataset Information

Dataset Characteristics:
- 82 respondents
- Multiple academic courses
- Gender and year-based segmentation
- Monthly allowance and spending data
- Expense tracking behavior
- Risk level classification

Variables Included:
- Course
- Gender
- Year of Study
- Monthly Allowance
- Monthly Spending
- Savings
- Expense Tracking
- Payment Method
- Food Expenses
- Risk Level

---

## DAX Measures Implemented

Key DAX measures used in the project include:

```DAX
Total Spending = SUM('Student Data'[Monthly_Spending])

Avg Allowance = AVERAGE('Student Data'[Monthly_Allowance])

Avg Savings = AVERAGE('Student Data'[Savings])

Savings Rate =
DIVIDE(
    SUM('Student Data'[Savings]),
    SUM('Student Data'[Monthly_Allowance])
) * 100
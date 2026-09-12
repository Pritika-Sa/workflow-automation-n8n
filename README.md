# 🎓 Autonomous Student Academic Advisory & Early Warning System

An automated academic monitoring and early warning system built using **n8n Workflow Automation** to identify students who may be at academic risk and support timely intervention.

## 📌 Project Overview

The system analyzes student academic data such as attendance, GPA, midterm performance, credits completed, and course difficulty.

Based on predefined academic thresholds, each student is assigned a **Risk Score** and classified into:

- 🟢 Low Risk
- 🟡 Medium Risk
- 🔴 High Risk

The system also identifies weak subjects and generates appropriate academic recommendations.

## 🎯 Objectives

- Automate student academic performance monitoring
- Identify academically at-risk students at an early stage
- Provide an explainable risk assessment
- Identify weak academic subjects
- Generate personalized intervention recommendations
- Automatically notify academic advisors

## 🔄 Workflow

```text
Google Sheets
     ↓
Get Student Records
     ↓
Validate Student Data
     ↓
Academic Risk Assessment
     ↓
Risk Classification
     ↓
   ┌───────────────┐
   │               │
 Low Risk      Medium/High Risk
   │               │
   ↓               ↓
Build Record   Build Full Record
   │               │
   ↓               ↓
    Save Assessment
                   ↓
          AI Mentor Recommendation
                   ↓
             Notification Gate
                   ↓
             Advisor Alert

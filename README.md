<p align="center">
  <img src="https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white">
  <img src="https://img.shields.io/badge/Security-IAM-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/AZ--500-Aligned-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Privileged%20Identity%20Management-blue?style=for-the-badge">
</p>

<h1 align="center">🔐 Azure Privileged Identity Management (PIM) & IAM Hardening Lab</h1>

<p align="center">
Enterprise Identity Governance using Microsoft Entra ID  
Aligned with AZ-500 – Identity & Access Domain
</p>

---

# 🏗️ Lab Architecture Overview

<p align="center">
  <img src="screenshots/lab-architecture.png" width="90%">
  <br>
  <em>Figure 1 — PIM Architecture in Microsoft Entra ID (Eligible → Just-In-Time Active → Audit Logging)</em>
</p>

### Architecture Flow Explained

1. Test users are created inside the Microsoft Entra ID Student Tenant  
2. Users are assigned **Eligible** roles using Privileged Identity Management  
3. Role activation requires **justification (JIT elevation)**  
4. Activation transitions from Eligible → Active  
5. All privileged activity is logged in Azure Activity Logs  

This simulates real-world enterprise identity governance.

---

# 🎯 Lab Objective

This lab demonstrates secure privileged access management using:

- Eligible role assignments  
- Permanent eligible configuration  
- Just-in-time (JIT) activation  
- Mandatory justification  
- Audit log validation  

The objective is to apply **least privilege principles** and reduce standing administrative access.

---

# 🖼️ Implementation Evidence

## 1️⃣ Creating Entra ID Users

<p align="center">
  <img src="screenshots/Create User.png" width="85%">
  <br>
  <em>Figure 2 — Creating internal test users in Microsoft Entra ID</em>
</p>

---

## 2️⃣ Configuring Eligible Assignment (Permanent Eligible Enabled)

<p align="center">
  <img src="screenshots/temporty access create the users .png" width="85%">
  <br>
  <em>Figure 3 — Assigning User Administrator role as Eligible with Permanent Eligible enabled</em>
</p>

Key Configuration:
- Assignment Type: Eligible
- Role: User Administrator
- Permanent Eligible: Enabled
- Defined start & end date

---

## 3️⃣ Role Activation with Justification (JIT Access)

<p align="center">
  <img src="screenshots/temporty access.png" width="85%">
  <br>
  <em>Figure 4 — Just-in-Time role activation requiring justification</em>
</p>

Activation requires:
- Justification entry
- Time-bound activation
- Approval workflow (if configured)

---

# 📋 Implementation Steps Summary

1. Created test users in Microsoft Entra ID  
2. Navigated to Privileged Identity Management → Microsoft Entra Roles  
3. Assigned **User Administrator** as Eligible  
4. Enabled **Permanent Eligible** option  
5. Activated role using Just-in-Time access  
6. Verified status under Activity Details  

---

# 🔐 Security Principles Demonstrated

✔ Least Privilege  
✔ Just-in-Time (JIT) Elevation  
✔ Role Governance  
✔ Audit & Accountability  
✔ Zero Trust Identity Model  

---

# 🧠 Key Learnings

- Difference between **Eligible vs Active** role assignments  
- Why permanent admin access increases risk  
- How PIM reduces attack surface  
- Importance of justification & logging for compliance  
- Enterprise IAM hardening strategies  

---

# 🎓 AZ-500 Certification Alignment

This lab supports:

- Implement identity governance  
- Configure privileged access  
- Manage Microsoft Entra roles  
- Monitor privileged activity  

---

# 🏛 Enterprise Security Value

In real-world organizations:

Uncontrolled administrative access is a major breach vector.

Using PIM:
- Standing admin access is eliminated  
- Privileges are time-bound  
- All elevation is logged  
- Governance & compliance posture improves  

---

# 👨‍💻 Author

**Amal Udayanga Basnayake**  
Cloud Security | Azure Security | Identity & Access Governance  

🔗 LinkedIn: https://www.linkedin.com/in/amal-udayanga-basnayake  
🔗 GitHub: https://github.com/AmalUBasnayake  

---

<p align="center">
⭐ If this lab supports your AZ-500 preparation, consider starring the repository!
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white">
  <img src="https://img.shields.io/badge/Security-IAM-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/AZ--500-Aligned-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Privileged%20Identity%20Management-blue?style=for-the-badge">
</p>

 <p align="center">
  <a href="https://github.com/AmalUBasnayake/Azure-IAM-PIM-Lab/stargazers">
    <img src="https://img.shields.io/github/stars/AmalUBasnayake/Azure-IAM-PIM-Lab?style=social">
  </a>
  <a href="https://www.linkedin.com/in/amal-udayanga-basnayake">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin">
  </a>
  <a href="https://github.com/AmalUBasnayake">
    <img src="https://img.shields.io/badge/GitHub-Portfolio-black?style=flat&logo=github">
  </a>
</p>

<h1 align="center">🔐 Azure Privileged Identity Management (PIM) & IAM Hardening Lab</h1>

<p align="center">
Enterprise Identity Governance using Microsoft Entra ID  
Aligned with AZ-500 – Identity & Access Domain
</p>

---

## 🎯 Lab Objective

This lab demonstrates secure identity and privileged access governance using:

✔ Role eligibility  
✔ Permanent eligible settings  
✔ Just-In-Time (JIT) activation with justification  
✔ Audit and activity tracking  

By enforcing least privilege and just-in-time access, this configuration strengthens identity security in Microsoft Entra ID (Azure AD).

---

## 🏗️ Architecture Overview

<p align="center">
  <img src="screenshots/Architecture.png" width="90%">
  <br><em>Figure 1 — PIM architecture showing eligible role assignment and JIT activation in Microsoft Entra ID.</em>
</p>

This diagram illustrates:

- Users created in Microsoft Entra ID  
- Eligible role assignments via PIM  
- Activation workflow requiring justification  
- Privileged role elevation to Active status  
- Audit logging for compliance

---

## 🖼️ Lab Output: Screenshots & Evidence

---

### 1️⃣ Creating Entra ID Users

<p align="center">
  <img src="screenshots/Create User.png" width="85%">
  <br><em>Figure 2 — Internal users created in Microsoft Entra ID.</em>
</p>

Users were created inside the tenant to simulate organizational identities.

---

### 2️⃣ Eligible Role Assignment (Permanent Eligible)

<p align="center">
  <img src="screenshots/temporty access create the users .png" width="85%">
  <br><em>Figure 3 — Setting User Administrator role as Eligible (Permanent eligible option enabled).</em>
</p>

Key settings:
✔ Role: User Administrator  
✔ Assignment Type: Eligible  
✔ Permanent Eligible: Yes

---

### 3️⃣ JIT Role Activation with Justification

<p align="center">
  <img src="screenshots/temporty access.png" width="85%">
  <br><em>Figure 4 — Activating privileged role with justification requirement.</em>
</p>

This ensures that privileged access is justified, audit-ready, and time-limited.

---

## 📋 Step-by-Step Implementation

1. Created test user accounts in Microsoft Entra ID  
2. Opened Privileged Identity Management → Microsoft Entra roles  
3. Assigned **User Administrator** role as Eligible  
4. Enabled “Permanent eligible” on the assignment  
5. Defined start & end dates  
6. Activated role with justification  
7. Verified assignment under Activity Details

---

## 🔐 Security Concepts Demonstrated

✔ Least Privilege Access  
✔ Just-In-Time (JIT) Elevation  
✔ Eligible vs Active Role States  
✔ Audit & Accountability  
✔ Identity Governance & Compliance

---

## 🧠 Key Learnings

- Eligible assignments provide controlled access without standing privileges  
- Justification and logging support compliance requirements  
- Permanent eligible assignments simplify repeated admin access
- PIM encourages Zero Trust identity practices

---

## 🎓 AZ-500 Certification Relevance

This lab supports these AZ-500 objectives:

✔ Implement identity governance  
✔ Manage privileged access  
✔ Monitor role activations  
✔ Configure PIM for least privilege  

---

## 🏛 Enterprise Security Value

In real-world environments, uncontrolled admin access is a serious risk factor for:

⚠ Insider threats  
⚠ Account takeover attacks  
⚠ Security misconfigurations  
⚠ Compliance failures

Implementing PIM with just-in-time activation reduces risk and improves governance.

---

## 👨‍💻 About the Author

**Amal Udayanga Basnayake**  
Cloud Security | Azure Security Engineer | Identity & Access Governance

🔗 LinkedIn: https://www.linkedin.com/in/amal-udayanga-basnayake  
🔗 GitHub: https://github.com/AmalUBasnayake  

<p align="center">
⭐ If this lab helped your AZ-500 prep, consider giving the repository a star!
</p>

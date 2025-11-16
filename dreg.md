# 🛡️ Microsoft Entra
## 🎯 Scenario: Block Device Code Flow

**Background:**  

An accountancy firm wants to ensure only trusted devices and authenticated users can access sensitive financial data

---

## ✅ Lab Objective  

To strengthen security by enforcing all users to register devices using MFA across the Microsoft 365 environment.

---

## 🧩 Step-by-Step Instructions

### Step 1: Setup policy

Go to the Entra portal and select **Entra ID > Conditional Access > New Policy**. Name the policy and select All users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cc36b754a78a1e48682cf3c3b74c2865fcc2ccb5/DR1.png" />

---

### Step 2: Exclude break glass account

Ensure break glass account is excluded to prevent lockout and for emergency access. 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cc36b754a78a1e48682cf3c3b74c2865fcc2ccb5/DR2.png" />

---

### Step 3: Add target resource policy

Select the policy to apply to **User Actions** and select **Register or join devices**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cc36b754a78a1e48682cf3c3b74c2865fcc2ccb5/DR3.png" />

---

### Step 4: Add Access control 

Configure policy by selecting **Grant > Grant access** after select **Require authentication strength** and **Multicator Authentication**. After **Enable policy** and select **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cc36b754a78a1e48682cf3c3b74c2865fcc2ccb5/DR4.png" />

---




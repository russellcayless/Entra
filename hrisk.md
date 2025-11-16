# 🛡️ Microsoft Entra
## 🎯 Scenario: Block High Risk Sign Ins 

**Background:**  

An accountancy firm want to block high-risk sign-ins to ensure client financial data is only accessed from trusted locations and secure accounts, reducing the risk of fraud or breaches.

---

## ✅ Lab Objective  

Using conditional access ensure that high-risk sign-ins and insecure authentication methods are blocked to protect sensitive financial data.

---

## 🧩 Step-by-Step Instructions

### Step 1: Setup policy

Go to the Entra portal and select **Entra ID > Conditional Access > New Policy**. Name the policy and select All users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/91a0d60b2c3be3ffa1890b52e83bfc19a1e613f6/Leg1.png" />

---

### Step 2: Exclude break glass account

Ensure break glass account is excluded to prevent lockout and for emergency access. 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/7be68fd604fab1da5fb0756481598aab49066685/Leg5.png" />

---

### Step 3: Add condition to policy

Select policy to include **Conditions > Client apps** and select **Yes** to configure and de-select **Browser, Mobile apps and Desktop clients**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/91a0d60b2c3be3ffa1890b52e83bfc19a1e613f6/Leg3.png" />

---

### Step 4: Add Access Controls to policy

Configure policy by selecting **Grant > Block access** after **Enable policy** and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/91a0d60b2c3be3ffa1890b52e83bfc19a1e613f6/Leg4.png" />

---




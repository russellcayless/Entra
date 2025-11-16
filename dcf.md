# 🛡️ Microsoft Entra
## 🎯 Scenario: Block Device Code Flow

**Background:**  

An accountancy firm identified that several user accounts lacked multi-factor authentication (MFA), leaving them vulnerable to credential theft and unauthorized access attempts.

---

## ✅ Lab Objective  

To strengthen account security by enforcing multi-factor authentication for all users across the Microsoft 365 environment.

---

## 🧩 Step-by-Step Instructions

### Step 1: Setup policy

Go to the Entra portal and select **Entra ID > Conditional Access > New Policy**. Name the policy and select All users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_user.png" />

---

### Step 2: Exclude break glass account

Ensure break glass account is excluded to prevent lockout and for emergency access. 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_user_ex.png" />

---

### Step 3: Add resources to policy

Select policy to include **All resources**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_resource.png" />

---

### Step 4: Add network location to policy

Configure policy to include **Any network or location**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_network_in.png" />

---

### Step 5: Add network exclusion to policy

Exclude **All trusted networks and locations**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_user_in.png" />

---




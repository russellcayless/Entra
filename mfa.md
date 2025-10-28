# 🛡️ Microsoft Entra
## 🎯 Scenario: MFA all users

**Background:**  

An accountancy firm identified that several user accounts lacked multi-factor authentication (MFA), leaving them vulnerable to credential theft and unauthorized access attempts.

---

## ✅ Lab Objective  

To strengthen account security by enforcing multi-factor authentication for all users across the Microsoft 365 environment.

---

## 🧩 Step-by-Step Instructions

### Step 1: Add countries locations

Go to the Entra portal and select **Entra ID > Conditional Access > Named Locations > Countries Location**. Enter name of location. Select **Include unknown countries/regions** and all countries. Search for Unitied Kingdom and de-select country. **Create** location. 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_user.png" />

---

### Step 2: Setup conditional access policy 

Select **Entra ID > Conditional Access > Policies > New Policy**. Name the policy and select **All users**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_user_ex.png" />

---

### Step 3: Add resources to policy

Select policy to include **All resources**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_resource.png" />

---

### Step 4: Add network location to policy

Configure policy to include **Select networks and locations** and select **All countries except UK**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_network_in.png" />

---

### Step 5: Add acceess controls

Select **Grant** control access and set to **Block access**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_user_in.png" />

---

### Step 6: Enable policy 

Turn on policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_grant.png" />

---

### Step 6: Enable policy 

Turn on policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5c7ee6b1caee46c1c76d91c3379791b82ca5a765/mfa_enable.png" />

---

### Step 6: Enable policy 

Turn on policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/main/mfa_test.png" />

---



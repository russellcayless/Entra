# 🛡️ Microsoft Entra
## 🎯 Scenario: Require Compliant Devices

**Background:**  

An accountancy firm wishes to ensure users are only accessing their data on devices that meet the organisations compliant security baseline.

---

## 🧩 Step-by-Step Instructions

### Step 1: Create Policy

Go to the Entra portal and select **Entra ID > Conditional Access > Create New Policy**, Name policy and assign to all users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/509c4e229b7d2a44505e8c47687f13ffe9e0cb7d/rcd1.png" />

---

### Step 2: Exclude group

Exclude the Break Glass group

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/509c4e229b7d2a44505e8c47687f13ffe9e0cb7d/rcd2.png" />

---

### Step 3: Target Resources

Select **Target Resources > All Resources** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/509c4e229b7d2a44505e8c47687f13ffe9e0cb7d/rcd3.png" />

---

### Step 4: Grant

Select **Grant > Require device to be marked as compliant** 

<img width="1767" alt="[Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/509c4e229b7d2a44505e8c47687f13ffe9e0cb7d/rcd4.png" />

---

### Step 5: Conditions

Select **Conditions > Device Platforms > Yes (to configure) > Include platforms currently using in organisation**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/509c4e229b7d2a44505e8c47687f13ffe9e0cb7d/rcd5.png" />

---

### Step 6: Enable Policy

Turn on Policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/509c4e229b7d2a44505e8c47687f13ffe9e0cb7d/rcd6.png" />

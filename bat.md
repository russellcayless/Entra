# 🛡️ Microsoft Entra
## 🎯 Scenario: Block Authentication Transfer

**Background:**  

An accountancy firm wishes to stop users being able to use cross device sign-in to reduce risk of tokens being obtained for malicious purposes.

---

## 🧩 Step-by-Step Instructions

### Step 1: Create Policy

Go to the Entra portal and select **Entra ID > Conditional Access > Create New Policy**, Name policy and assign to all users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/b3813c1b09b2deea174a326c8412e9f0b4fb8744/ca-bat1.png" />

---

### Step 2: Exclude group

Exclude the Break Glass group

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/b3813c1b09b2deea174a326c8412e9f0b4fb8744/ca-bat2.png" />

---

### Step 3: Target Resources

Select **Target Resources > All Resources** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/b3813c1b09b2deea174a326c8412e9f0b4fb8744/ca-bat3.png" />

---

### Step 4: Conditions

Select **Conditions > Authentication Flows > Yes (to configure) > Authentication Transfer**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/b3813c1b09b2deea174a326c8412e9f0b4fb8744/ca-bat4.png" />

---

### Step 5: Grant

Select **Grant > Block Access** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/b3813c1b09b2deea174a326c8412e9f0b4fb8744/ca-bat5.png" />

---

### Step 6: Enable Policy

Turn on Policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/b3813c1b09b2deea174a326c8412e9f0b4fb8744/ca-bat6.png" />

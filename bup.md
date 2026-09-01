# 🛡️ Microsoft Entra
## 🎯 Scenario: Block Unsupported Platforms

**Background:**  

An accountancy firm wishes to reduce exposure to platforms which it does not use within the organisation.

---

## 🧩 Step-by-Step Instructions

### Step 1: Create Policy

Go to the Entra portal and select **Entra ID > Conditional Access > Create New Policy**, Name policy and assign to all users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/dcf2a1a7454963b3b4ff8d6c5cde3ff99cc77ec5/ca-bup1.png" />

---

### Step 2: Exclude group

Exclude the Break Glass group

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/dcf2a1a7454963b3b4ff8d6c5cde3ff99cc77ec5/ca-bup2.png" />

---

### Step 3: Target Resources

Select **Target Resources > All Resources** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/dcf2a1a7454963b3b4ff8d6c5cde3ff99cc77ec5/ca-bup3.png" />

---

### Step 4: Conditions

Select **Conditions > Device Platforms > Yes (to configure) > Exclude platforms currently using in organisation**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/dcf2a1a7454963b3b4ff8d6c5cde3ff99cc77ec5/ca-bup4.png" />

---

### Step 5: Grant

Select **Grant > Block Access** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/dcf2a1a7454963b3b4ff8d6c5cde3ff99cc77ec5/ca-bup6.png" />

---

### Step 6: Enable Policy

Turn on Policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/dcf2a1a7454963b3b4ff8d6c5cde3ff99cc77ec5/ca-bup7.png" />

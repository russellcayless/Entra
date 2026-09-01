# 🛡️ Microsoft Entra
## 🎯 Scenario: Windows Token Protection

**Background:**  

An accountancy firm wants to enable Token Protection for Microsoft 365 to reduce the risk of attackers using stolen authentication tokens to access corporate data. If an employee's session token is stolen by malware or an infostealer, Token Protection helps prevent that token from being reused on another device to access services such as Exchange Online, SharePoint and Teams. This provides an additional layer of security beyond passwords and MFA, helping protect sensitive company emails, files and communications. 

---

## 🧩 Step-by-Step Instructions

### Step 1: Create Policy

Go to the Entra portal and select **Entra ID > Conditional Access > Create New Policy**, Name policy and assign to all users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w1.png" />

---

### Step 2: Exclude group

Exclude the Break Glass group

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w2.png" />

---

### Step 3: Target Resources

Select **Target Resources > Select Resources** and select **Microsoft Teams Services, Office 365 Sharepoint Online, Office 365 Exchange online**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w3.png" />

---

### Step 4: Conditions

Select **Conditions > Device Platforms > Yes (to configure) > Include > Windows**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w4.png" />

---

### Step 5: Conditions

Select **Conditions > Client Apps > Yes (to configure) > Include > Mobile apps and desktop clients**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w5.png" />

---

### Step 6: Session

Select **Session > Require token protection for sign-in sessions**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w6.png" />


---

### Step 7: Enable Policy

Turn on Policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/85978bbf45d85d008163b2eb1f8afa6b8a2072cd/ca-w7.png" />


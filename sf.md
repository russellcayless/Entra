# 🛡️ Microsoft Entra
## 🎯 Scenario: Sign-In Frequency & Session

**Background:**  

An accountancy firm wishes to ensure users and admins sessions are not permanently authenticated. They must regularly re-authenticate and not maintain a persistent browser session. 

---

## 🧩 Step-by-Step Instructions for Users

### Step 1: Create Policy

Go to the Entra portal and select **Entra ID > Conditional Access > Create New Policy**, Name policy and assign to all users

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC1.png" />

---

### Step 2: Exclude group

Exclude the Break Glass group

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC2.png" />

---

### Step 3: Target Resources

Select **Target Resources > All Resources** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC3.png" />

---

### Step 4: Conditions

Select **Conditions > Filter for devices > Yes (to configure) > IsCompliant-Equals-True**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC4.png" />

---

### Step 5: Session

Select **Session > Sign-in Frequency (7 Days) & Persistent Browser Session > Never Persistent**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC5.png" />

---

### Step 6: Enable Policy

Turn on Policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC6.png" />

---

## 🧩 Step-by-Step Instructions for Admins

### Step 1: Create Policy

Go to the Entra portal and select **Entra ID > Conditional Access > Create New Policy**, Name policy & Select **Directory Roles > Admins (Cloud Application, Conditional Access, Exchange, Global, Helpdesk, Security, Sharepoint, User)**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC7.png" />

---

### Step 2: Exclude group

Exclude the Break Glass group

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC8.png" />

---

### Step 3: Target Resources

Select **Target Resources > All Resources** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC9.png" />

---

### Step 4: Session

Select **Session > Sign-in Frequency (4 Days) & Persistent Browser Session > Never Persistent**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/SC10.png" />

---

### Step 5: Enable Policy

Turn on Policy and **Create**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/118401fc8f2bc17a7f6e4051242a0196d9eb137f/sc11.png" />





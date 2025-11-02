# 🛡️ Microsoft Entra
## 🎯 Scenario: Basic password protection & SSPR

**Background:**  

An accountancy firm required stronger password controls and a secure, user-friendly password reset process to reduce helpdesk workload and improve account security.

---

## ✅ Lab Objective  
By branding your organization’s Microsoft 365 sign-in experience, users can visually confirm they are on the real company login portal:

- Add countries locations to include UK as trusted site
- Setup conditional access policy to block all countries except UK
- Use a VPN connection to simulate a sign-in from a non-UK location.
- Create a security group in Entra ID for approved exception users.
- Test exception, reattempt the sign-in from a non-UK VPN location and confirm the user is allowed access as expected.

---

## 🧩 Step-by-Step Instructions

### Step 1: Custom banned password list

Obtain list of common banned passwords used. 

<img width="500" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass2.png" />

---

### Step 2: Set Password Protection

Select **Entra ID**. Search for **Password Protection**. Configure following settings and **Save**

- Lockout Theshold - **5**
- Lockout duration in seconds - **30**
- Enforce custom List - **Yes**
- Custom banned password list - **Add passwords**
- Mode - **Enforced** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass1.png" />

---

### Step 3: Password Reset Settings

Search for **Password Reset** Enable all users and **Save**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass3.png" />

---

### Step 4: Registration

Select **Registration** and set to **Yes** for users to register when signing-in. Set number of days to **90** for users to re-confirm their authentication. **Save**
 
<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass4.png" />

---

### Step 5: Notifications

Select **Yes** for notifying users and admins when passwords are reset.**Save**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass5.png" />

---

### Step 6: Authentication Methods

To increase security set number of methods required to reset to **2** and **Save.** Select link to view **auth methods policy**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass6.png" />

---

### Step 7: Auth Methods

Enable following auth methods:

- Passkey (FIDO2)
- Microsoft Authenticator 
- Tempoary Access Pass
- Software OATH tokens
- Email OTP

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/cb19849dc06d59278135fe52b8a62d175ad94d30/pass7.png" />

---

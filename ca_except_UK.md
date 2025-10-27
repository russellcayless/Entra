# 🛡️ Microsoft Entra
## 🎯 Scenario: Block all countries except UK

**Background:**  

An accountancy firm identified multiple unauthorized sign-in attempts originating from foreign IP addresses. To reduce the risk of account compromise, a geolocation-based access control policy was required.

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

### Step 1: Add countries locations

Go to the Entra portal and select **Entra ID > Custom Branding > Default sign-in > Edit**. This is where you can upload a company background image.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/3e39090f4c9e6383cf55ffce43096ababdb18183/named_location.png" />

---

### Step 2: Setup conditional access policy 

Select **Layout** prefered menu behaviour **Template / Header / Footer**. In this example **Partial-screen background** has been selected instead of traditional full screen. 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/layout.png" />

---

### Step 3: Add resources to policy

Select **Sign-in form** then upload logos **Banner / Square (light + dark)** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/banner.png" />
<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/squarelogo.png" />
<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/squarelogodark.png" />


---

### Step 4: Add network location to policy

Enter sign-in page text that you wish to display when users login. Then **Review + save**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/signintext.png" />

---

### Step 5: Add condition to policy 

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 6: Enable policy 

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 7: Enable VPN

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 8: Test sign-in is blocked

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 9: Create exception group 

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 10: Add member

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 11: Add group to policy

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

### Step 12: Test sign-in is successful

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

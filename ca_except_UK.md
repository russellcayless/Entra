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

### Step 1: Navigate to Microsoft Entra

Go to the Entra portal and select **Entra ID > Custom Branding > Default sign-in > Edit**. This is where you can upload a company background image.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/8cc64d8736d29b8cb65b06001833d98ebbacfae0/backgroundimage.png" />

---

### Step 2: Visual Templates

Select **Layout** prefered menu behaviour **Template / Header / Footer**. In this example **Partial-screen background** has been selected instead of traditional full screen. 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/layout.png" />

---

### Step 3: Configure logos on sign-in form

Select **Sign-in form** then upload logos **Banner / Square (light + dark)** 

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/banner.png" />
<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/squarelogo.png" />
<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/squarelogodark.png" />


---

### Step 4: Add Sign-in page text

Enter sign-in page text that you wish to display when users login. Then **Review + save**

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/signintext.png" />

---

### Step 5: Confirm login page is branded 

Login as user to confirm that changes have now been implemented.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/russellcayless/Entra/blob/5182cf817bead3c64688aef5d6381b59829bf5c9/brandedloginscreen.png" />

---

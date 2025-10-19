# 🛡️ Microsoft Purview Endpoint DLP Lab  
## 🎯 Scenario: Insider Risk - Employee Attempts to Exfiltrate Sensitive Data in ZIP File

**Background:**  
A contractor working remotely downloads sensitive customer financial data to their local machine and archives it in a ZIP file for "backup." They then attempt to upload the ZIP file to a personal cloud service (e.g., Dropbox or Google Drive) from a corporate-issued device. The organization must detect and prevent this potential data exfiltration.

---

## ✅ Lab Objective  
Simulate the detection and prevention of sensitive data (e.g., SSNs, financial records) stored in archive files on an Entra-joined Windows 10/11 VM.  
Create a custom Microsoft Purview Endpoint DLP policy to block actions such as:

- Uploading sensitive files to cloud services
- Copying to clipboard
- Attempting unauthorized transfers

---

## 🧩 Step-by-Step Instructions with Explanations

### Step 1: Navigate to Microsoft Purview DLP

Go to the Microsoft Purview portal and select **Data Loss Prevention > Policies**. This is where all existing and new policies can be managed.

<img width="1767" alt="Screen Shot 2025-05-07 at 11 26 51 PM" src="https://github.com/user-attachments/assets/da69c38e-97b3-4f7b-9b8b-e6cab79fdd33" />

---


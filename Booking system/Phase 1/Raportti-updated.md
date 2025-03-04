# Penetration Testing Report
   ## Updated 4.3.2025! ##
## 1. Introduction  
    
### Purpose and Scope of the Report
This report presents the findings of a penetration test conducted on the Booking System web application. The purpose of this assessment is to identify security vulnerabilities that could be exploited by attackers and provide recommendations for remediation.

### Testing Schedule and Environment
- **Testing Period:** 17-20.2.2025 (Retested 3.3.2025)
- **Environment:** The test was conducted on a locally hosted website in a virtual machine environment (`http://localhost:8000`).
- **Operating System:** Kali Linux
- **Target Scope:** User registration

### Methods and Tools Used for Testing
- **Testing Approach:** Grey-box testing
- **Tools Used:**
  - OWASP ZAP (HAR method)
  - Dirb
  - Nikto
  - Nmap (realized I was scanning my own computer ports, doesn't work on VM locally hosted apps)

---

## 2. Summary

### Key Findings and Recommendations

#### 1. **SQL Injection (Critical - Fixed)**
   - The registration form was previously vulnerable to SQL injection, but this issue has been resolved in the latest version.
   - **Status:** Fixed.

#### 2. **Lack of Security Headers (Medium - Fixed)**
   - Missing Content Security Policy (CSP) and Clickjacking protection headers have been implemented.
   - **Status:** Fixed.

#### 3. **Error Message Disclosure (Low - Fixed)**
   - Stack traces and database error messages are no longer visible to users.
   - **Status:** Fixed.

#### 4. **X-Content-Type-Options Header Missing (Low - Fixed)**
   - The `X-Content-Type-Options` header is now set to `nosniff`.
   - **Status:** Fixed.

### General Assessment of Security State
The system has shown significant improvement in its security posture. All previously identified vulnerabilities have been addressed, and no new critical, medium, or low vulnerabilities were found in the latest ZAP scan. The application now demonstrates consistent behavior across different User-Agent strings, as confirmed by the User Agent Fuzzer test.

---

## 3. Findings and Categorization

### **Critical Vulnerabilities**

#### **SQL Injection in Registration Form (Fixed)**
   - **Vulnerable Parameters:** `username`
   - **Impact:** Previously allowed attackers to manipulate database queries, potentially compromising the entire system.
   - **Status:** Fixed. Parameterized queries and input validation have been implemented.

### **Medium Vulnerabilities**

#### **Missing Content Security Policy (CSP) (Fixed)**
   - **Impact:** Previously increased the risk of Cross-Site Scripting (XSS) attacks.
   - **Status:** Fixed. The `Content-Security-Policy` header has been added.

#### **Missing Anti-clickjacking Header (Fixed)**
   - **Impact:** Previously allowed attackers to trick users into clicking unintended elements.
   - **Status:** Fixed. The `X-Frame-Options: DENY` header has been implemented.

### **Low Vulnerabilities**

#### **Application Error Disclosure (Fixed)**
   - **Impact:** Previously revealed potentially exploitable system details.
   - **Status:** Fixed. Custom error pages have been implemented.

#### **X-Content-Type-Options Header Missing (Fixed)**
   - **Impact:** Previously increased the risk of MIME-type sniffing attacks.
   - **Status:** Fixed. The `X-Content-Type-Options: nosniff` header has been added.

### **Informational Findings**

#### **User Agent Fuzzer**
   - **Description:** ZAP tested the application with various User-Agent strings to detect differences in responses.
   - **Impact:** No significant issues were found. The application behaves consistently across different User-Agent strings.
   - **Recommendation:** Ensure the application continues to behave consistently regardless of the User-Agent string.

---

## 4. Appendices

### ZAP-report-v1
### Zap-report-v2

### Nikto Output
![image](https://github.com/user-attachments/assets/55211b0d-a977-4c08-bf8f-a117f13995e7)

### SQL Password Not Encrypted (Fixed)
![image](https://github.com/user-attachments/assets/39edf13d-69c5-4de5-bcce-b481b3516c5a)
![image](https://github.com/user-attachments/assets/f5275fa7-81fe-45bc-a05a-527add594ea2)


### No Input Validation (Fixed)
![image](https://github.com/user-attachments/assets/917d5bdd-7727-4494-a564-cae86b679585)
![image](https://github.com/user-attachments/assets/c40b5295-f87a-46a1-95c9-fb4296965c2c)


### Error Message Giving Potentially Confidential Information (Fixed)
![image](https://github.com/user-attachments/assets/3baa4a2b-a385-4b13-915f-f8a33e8ba1c6)

### Dirb Scan Results (No Hidden Files Found)
![image](https://github.com/user-attachments/assets/0dd73908-3931-4b97-b3cd-e2641aa965f4)
![image](https://github.com/user-attachments/assets/5e970838-c1c5-446e-b7c7-1290f388be2c)

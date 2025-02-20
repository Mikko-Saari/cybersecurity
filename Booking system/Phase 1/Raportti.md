# Penetration Testing Report

## 1. Introduction

### Purpose and Scope of the Report

This report presents the findings of a penetration test conducted on the Booking System web application. The purpose of this assessment is to identify security vulnerabilities that could be exploited by attackers and provide recommendations for remediation.

### Testing Schedule and Environment

- **Testing Period:** 17-20.2.2025
- **Environment:** The test was conducted on a locally hosted website in a virtual machine environment (`http://localhost:8000`).
- **Operating System:** Kali Linux
- **Target Scope:** User registration

### Methods and Tools Used for Testing

- **Testing Approach:** Grey-box testing
- **Tools Used:**
  - OWASP ZAP (HAR method)
  - Dirb
  - Nikto
  - Nmap (realized I was scanning my own computer ports)

---

## 2. Summary

### Key Findings and Recommendations

#### 1. **SQL Injection (Critical - Immediate Fix Required)**
   - The registration form is vulnerable to SQL injection, allowing attackers to manipulate database queries.
   - **Recommendation:** Implement prepared statements and input validation. Type check all data on the server side.

#### 2. **Lack of Security Headers (Medium - Fix Recommended Soon)**
   - Missing Content Security Policy (CSP) and Clickjacking protection headers.
   - **Recommendation:** Configure HTTP headers to enhance security.

#### 3. **Error Message Disclosure (Low - Should Be Addressed)**
   - Stack traces and database error messages are visible, revealing sensitive data.
   - **Recommendation:** Implement custom error pages.

### General Assessment of Security State

The system has significant security vulnerabilities, the most severe being SQL injection, which puts the entire application at risk. The lack of security headers enables Clickjacking attacks, potentially leading to unauthorized access to user information. Additionally, error messages disclose too much information, which could be exploited. Immediate action is required to secure the website and it's users.

---

## 3. Findings and Categorization

### **Critical Vulnerabilities**

#### **SQL Injection in Registration Form**
   - **Vulnerable Parameters:** `username` and `password`
   - **Impact:** Allows attackers to manipulate database queries, potentially compromising the entire system.
   - **Recommended Fix:** Use parameterized queries, never trust client-side input, and validate input on the server side using regex.

### **Medium Vulnerabilities**

#### **Missing Content Security Policy (CSP)**
   - **Impact:** Increases risk of Cross-Site Scripting (XSS) attacks.
   - **Recommended Fix:** Add `Content-Security-Policy` headers.

#### **Missing Clickjacking Protection**
   - **Impact:** Attackers can trick users into clicking unintended elements, potentially revealing confidential data (e.g., username, password).
   - **Recommended Fix:** Implement `X-Frame-Options: DENY` to prevent the application from being loaded inside an iframe.

### **Low Vulnerabilities**

#### **Application Error Disclosure**      
   - **Impact:** Reveals potentially exploitable system details.
   - **Recommended Fix:** Implement custom error pages.

#### **X-Content-Type-Options Header Missing**
   - **Impact:** Increases risk of MIME-type sniffing attacks.
   - **Recommended Fix:** Configure the web server to send the `X-Content-Type-Options: nosniff` header.

---

## 4. Appendices



Nikto output:
![image](https://github.com/user-attachments/assets/55211b0d-a977-4c08-bf8f-a117f13995e7)


SQL password is not crypted
![image](https://github.com/user-attachments/assets/39edf13d-69c5-4de5-bcce-b481b3516c5a)

How it could/should look like
![image](https://github.com/user-attachments/assets/a28ed709-d1d8-4937-af80-cf1fde735e68)

No input validation/no validation of any kind 

![image](https://github.com/user-attachments/assets/917d5bdd-7727-4494-a564-cae86b679585)


Error message giving potentially confidental information

![image](https://github.com/user-attachments/assets/3baa4a2b-a385-4b13-915f-f8a33e8ba1c6)


Scanning for hidden files with dirb, didint find anything.
![image](https://github.com/user-attachments/assets/0dd73908-3931-4b97-b3cd-e2641aa965f4)


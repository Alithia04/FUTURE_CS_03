# FUTURE_CS_03
API Security Analysis
 ## Overview
 This project focuses on performing an API Security Risk Analysis using a public demo API. 
 The objective of the assessmnet was to identify common API security risks, evaluate authentication and response handling and provide remediation recommendations using safe and ethical testing methods. 
----
## API Tested
JSONPlaceholder Test API

Base URL 
https://jsonplaceholder.typicode.com

Endpoint Tested: 
https://jsonplaceholder.typicode.com/users

--- 

##Methodology
The following steps were performed during the assessment: 

- Sent read-only GET requests
- Inspected API reponse headers
- Ana;yzed API reponse body data revied authentication requiremnets
- Evaluated information diclosure risks
- Checked rate limiting behavior
No explotation or destructive testing was performed.

----

## Security Findings

### 1. No Authenticattion Required
The API endpoint was accessble without authentication or API keys.

**Severity:** Medium
----
### 2. Excessive Data Exposure
The API response exposed user information including:
- Email addresses
- Phone numbers
- Addresses
- Company inforamtion
- 
  **Severity:** Medium

  ----
  ### 3. Server Technology Disclosure
  The reponse headers revealed backend technology information through:
  - x-powered-by: Express
  
    **Severity:** Low

  ----

  ### 4. Missing Security Header
  Several recommended security headers were not observed during testing
  
  **Severity:** Low

  ----

  ### 5. Rate Limiting Implemented
  The API included rate limiting headers such as:
  - x-ratelomit-limit
  -  x-ratelimit-remaining
  - 
 This was identified as a positive security control
----

## ETHICAL NOTICE
This assesment was conducted ethically using safe and read-only testing methods.
No exploitation, denial-of-service attacks or unauthorized access attempts were performed. 

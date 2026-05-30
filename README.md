# FUTURE_CS_03
# API Security Risk Analysis

## Prepared By

**Deney Dasari**
**CIN ID:** FIT/MAY26/CS8415

## Internship

Future Interns – Cyber Security Internship

## Task

Cyber Security Task 3 (2026) – API Security Risk Analysis

## API Tested

JSONPlaceholder Test API

API URL:
https://jsonplaceholder.typicode.com

## Objective

The objective of this assessment was to analyze a public API, identify common API security risks, evaluate authentication and access control mechanisms, and provide remediation recommendations.

## Tools Used

* Postman
* Browser Developer Tools
* GitHub

## Scope

* Documentation Review
* Endpoint Testing
* Header Inspection
* Response Analysis
* Security Risk Identification

## Methodology

1. Reviewed API documentation.
2. Tested API endpoints using Postman.
3. Inspected response headers and data.
4. Identified potential security risks.
5. Assessed risk severity.
6. Provided remediation recommendations.

## Endpoints Tested

* GET /users
* GET /posts
* GET /users/1

## Findings

### Finding 1: Missing Authentication

**Severity:** Medium

The `/users` endpoint returned data without requiring authentication, API keys, or access tokens.

### Finding 2: Excessive Data Exposure

**Severity:** Medium

The API response exposed user information such as name, email, address, phone number, and website.

### Finding 3: Rate Limiting Implemented

**Severity:** Informational

Response headers contained rate-limiting controls including:

* x-ratelimit-limit
* x-ratelimit-remaining
* x-ratelimit-reset

### Finding 4: Predictable Resource IDs

**Severity:** Low

Resources were accessible through sequential numeric identifiers such as `/users/1`.

## Repository Structure

```text
report/
└── API_Security_Risk_Analysis_Report_Deney.pdf

screenshots/
├── users_endpoint.png
├── headers.png
└── user1_endpoint.png
```

## Disclaimer

This assessment was conducted on a public test API for educational purposes only. No unauthorized access, exploitation, or disruptive testing was performed.

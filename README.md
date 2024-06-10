# Vulnerability Assessment Report

**Date:** 31st May 2024

## System Description

The server features a robust CPU and 128GB of RAM. It operates on the latest Linux OS and runs a MySQL database management system. The server maintains a stable network connection via IPv4 addresses and communicates with other servers on the network. Security protocols include SSL/TLS encrypted connections.

## Scope

This vulnerability assessment focuses on the system's current access controls. It spans three months, from June 2023 to August 2023, and follows the guidelines of NIST SP 800-30 Rev. 1 for risk analysis.

## Purpose

The database server is a centralized computer system that stores and manages large amounts of data. The server is used to store customer, campaign, and analytic data that can later be analyzed to track performance and personalize marketing efforts. It is critical to secure the system because of its regular use for marketing operations.

## Risk Assessment

| Threat Source | Threat Event                              | Likelihood | Severity | Risk |
|---------------|-------------------------------------------|------------|----------|------|
| Hacker        | Obtain sensitive information via exfiltration | 3          | 3        | 9    |
| Employee      | Disrupt mission-critical operations        | 2          | 3        | 6    |
| Customer      | Alter/Delete critical information          | 1          | 3        | 3    |

## Approach

The risks assessed took into account the business's data storage and management practices. Potential threats and events were identified based on the likelihood of a security incident due to the system's open access permissions. The severity of these incidents was evaluated in terms of their impact on daily operations.

## Remediation Strategy

Sure, here's a reworded version of the list of remedies:

---

- Implement authentication, authorization, and auditing mechanisms to ensure only authorized users can access the database server.
- Utilize strong passwords, role-based access controls, and multi-factor authentication to restrict user privileges.
- Encrypt data in transit using TLS instead of SSL.
- Implement IP allow-listing to corporate offices to block unauthorized internet users from connecting to the database.

---

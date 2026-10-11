# Cybersecurity Course Project

**Topic:** Social Engineering, Malware Threats, and SQL Injection  
**Author:** Radoslav Valchev  
**Year:** 2026  
**Field of study:** Cybersecurity

## Overview

This repository contains a university course project covering three related cybersecurity topics:

- **Social engineering:** phishing, spear phishing, vishing, pretexting, baiting, examples, and defensive practices.
- **Malware:** viruses, worms, Trojan horses, ransomware, spyware, adware, rootkits, common delivery methods, and mitigation.
- **SQL injection:** a documented test of a web application's login form, stock-symbol input, and URL parameters. The report records the test inputs and the responses observed during the exercise.

The project emphasizes how human behavior and technical weaknesses can combine to create security risks, and why prevention requires both user awareness and technical controls.

## Repository structure

```text
cybersecurity-course-project/
├── README.md
├── docs/
│   └── course-project-report-bg-public-copy.docx
├── social-engineering/
│   └── README.md
├── malware/
│   └── README.md
└── sql-injection/
    └── README.md
```

## Main findings documented in the report

- The tested login form rejected the classic `' OR 1=1 --` input and a `UNION SELECT` test string with a normal authentication error.
- The “Add Stock” field rejected the test input with the message “We do not support this stock”.
- Modified URL parameters resulted in a 404 response.
- These observations did **not** demonstrate successful SQL injection during the documented tests. They are observations from the tested inputs, not proof that the entire application is free of vulnerabilities.

## Defensive measures discussed

- User awareness and verification of unexpected requests.
- Strong, unique passwords and multi-factor authentication.
- Antivirus/endpoint protection and firewalls.
- Timely operating-system and application updates.
- Caution with email attachments, links, downloads, and removable media.
- Backups, access controls, security policies, and training.
- Parameterized queries and safe database access patterns for SQL injection prevention.

## Report

The full Bulgarian report is included in `docs/`. A public-facing copy is provided; the student number and the tested host IP have been redacted to reduce unnecessary disclosure.

## Responsible-use note

The SQL injection section is a learning exercise. Only test systems that you own or have explicit permission to assess. Do not use the example payloads against third-party systems without authorization.

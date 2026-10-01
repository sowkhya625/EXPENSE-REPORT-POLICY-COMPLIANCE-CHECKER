<img width="1541" height="560" alt="Screenshot 2026-10-01 151236" src="https://github.com/user-attachments/assets/28455a1a-e487-476c-8ff4-12315994189c" />
## Expense Submission Form

Submit an expense receipt using the form:

[Open Expense Submission Form](https://forms.gle/tfdQLD2mP718cyXy7)
EXPENSE REPORT POLICY COMPLIANCE CHECKER
AI-Powered Receipt Verification and Compliance System
1. Introduction
The Expense Report Policy Compliance Checker is an AI-powered system designed to inspect scanned employee expense receipts and verify whether individual line items comply with company reimbursement policies. The system extracts receipt information using OCR, analyzes each expense against predefined rules, identifies potentially disallowed or suspicious items, and prepares a compliance summary before the expense report is routed to a manager.
2. Problem Statement
Manual expense verification is time-consuming and can lead to missed policy violations, inconsistent decisions, and delays in reimbursement. Organizations need an automated method to process receipts, validate expenses, highlight exceptions, and support managers during approval.
3. Objectives
•	Automatically extract information from scanned receipts.
•	Validate individual line items against company reimbursement rules.
•	Detect prohibited categories, excessive amounts, duplicate claims, and missing information.
•	Clearly explain why an expense has been flagged.
•	Generate a compliance summary for managers.
•	Maintain an audit trail of extracted data and verification results.
4. Proposed Workflow
Receipt Upload → OCR Extraction → Data Cleaning → Line-Item Classification → Policy Rule Check → Exception Detection → Compliance Report → Manager Review
5. System Modules
•	Receipt Upload Module: Accepts scanned images or PDF receipts.
•	OCR Module: Extracts merchant name, date, item descriptions, quantities, and amounts.
•	Expense Classification Module: Categorizes each line item such as meals, travel, accommodation, office supplies, or entertainment.
•	Policy Rule Engine: Applies company limits and reimbursement conditions.
•	AI Compliance Analyzer: Identifies unusual, ambiguous, or potentially non-compliant expenses.
•	Report Generator: Produces an itemized compliance result and summary.
•	Manager Review Module: Routes exceptions and reports for approval or further review.
6. Example Policy Checks
Expense	Example Rule	System Result
Business meal	Maximum ₹2,000 per employee	Flag if amount exceeds limit
Alcohol	Not reimbursable	Disallowed
Office supplies	Allowed within approved category	Allowed if policy conditions are met
Taxi/transport	Receipt and business purpose required	Review if information is missing
Duplicate receipt	Same receipt cannot be claimed twice	Flag as possible duplicate
7. Sample Output
Receipt: Restaurant Expense
Claimed Amount: ₹2,850
Policy Limit: ₹2,000
Status: NEEDS REVIEW
Reason: Expense exceeds the configured meal reimbursement limit by ₹850.
8. Technologies
•	Python for backend processing and automation.
•	OCR technology such as Tesseract or a cloud OCR service.
•	Natural Language Processing / Large Language Models for receipt and policy interpretation.
•	Rule-based policy engine for deterministic compliance checks.
•	Machine learning/anomaly detection for unusual expense patterns.
•	Flask or FastAPI for a web-based interface.
•	SQLite/MySQL/PostgreSQL for storing expense and audit information.
9. Advantages
•	Reduces manual verification effort.
•	Improves consistency in policy checking.
•	Provides transparent reasons for flagged expenses.
•	Helps managers focus on exceptions instead of checking every receipt manually.
•	Creates a searchable audit trail.
•	Can scale to large numbers of expense reports.
10. Future Enhancements
•	Integration with HR, accounting, and reimbursement platforms.
•	Multi-language and multi-currency receipt support.
•	Automatic duplicate and fraud-risk detection.
•	Role-based dashboards for employees, finance teams, and managers.
•	Continuous learning from approved and rejected expense cases, with human oversight.
11. Conclusion
The Expense Report Policy Compliance Checker provides an automated and explainable approach to expense verification. By combining OCR, AI-based document understanding, and deterministic policy rules, the system can identify potential violations before reports reach managers. This can reduce processing time while giving reviewers clear evidence and reasons for each flagged expense.

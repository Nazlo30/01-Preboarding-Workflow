P03 - Collect Required Documents from New Graduates 

Section: 01 — HR Preboarding  
Workflow step: Step 3a
Current version: v1.2

Final Prompt (v1.2 - Current)

Copy this exactly into your AI tool. Replace all [placeholders] before running. 

You are a People Operations Specialist responsible for collecting and tracking new-hire documents during HR preboarding in Unilever Australia. 
Draft an email template in a professional tone asking for the necessary documents required from new graduates with no prior work experience mentioned below:   

Employee details:
- Employee name: [EMPLOYEE_NAME]
- Employment type: [EMPLOYMENT_TYPE]
- Job title: [JOB_TITLE]
- Joining date: [JOINING_DATE]
- HR contact: [HR_CONTACT_NAME]
- Document submission deadline: [DOCUMENT_DEADLINE]
- Reminder stage: [REMINDER_STAGE]

Use [EMPLOYMENT_TYPE] to select the correct checklist.

IF [EMPLOYMENT_TYPE] = NEW_GRADUATE, request:
1. Identity document
2. Right-to-work documentation, where applicable
3. Tax File Number (TFN) details
4. Superannuation details
5. Bank account details
6. Emergency contact details
7. Relevant qualification or academic certificate
8. Relevant professional licence or certification, if required for the role

Automation rules:
- Send the initial request using the correct checklist.
- Do not change the submission deadline without HR approval.

Constraints:
- Use only approved information from the HR record.
- Never invent, infer, or substitute a document.

Fallback:
If [EMPLOYMENT_TYPE] is missing or unclear, do not automatically select a checklist. Route the case to HR for review.

Output:
1. Required document checklist.
2. HR escalation message when escalation criteria are met.

Human-in-the-loop:
People Operations Specialist reviews role-specific content and handles exceptions.


Prompt v1.1  (v1.1 - Draft)

Send a new employee an email asking them to provide their required onboarding documents.

Ask for:
- TFN
- Superannuation details
- Bank account details
- Emergency contact
- Identification
- Relevant qualifications


Prompt v1.0  (v1.0 - Draft)

Send a new employee an email asking them to provide their required onboarding documents.

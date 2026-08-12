HR Preboarding Workflow

Business function: Human Resources   
Business case: Unilever Australia 
Trigger:New hire receives final human hiring approval  


Section Purpose

These prompts support the repetitive administrative activities that occur between final hiring approval and the employee's first day. The library is designed around a connected workflow: each validated output becomes an input or trigger for the next step. Human review remains in place for employment decisions, exceptions, document inconsistencies, access approval, and identity-data errors.

Chain Diagram

```text
Candidate selected and approved
            |
            v
P01 · Send offer letter email
            |
            v
P02 · Manage offer letter response
            |
            v
P03 · Draft appointment letter
            |
            v
P04 · Appointment letter signature
            |
            v
     +------+------------------+
     |                         |
     v                         v
P05 · New Graduate       P06 · Experienced
      documents               employee documents
     |                         |
     +------------+------------+
                  |
                  v
P07 · Document collection reminders
                  |
                  v
P08 · Sync employee data to HR / Payroll
                  |
          +-------+--------+
          |                |
          v                v
P09 · IT device &     P10 · ID card
     email access           requisition
     requisition
```

## Human-in-the-Loop Points

| Step | Human action required |
|------|-----------------------|
| P01 output | Talent Advisor reviews the offer email and sends it to the employee. If there is an issue with the proposed joining date or job title, HR intervention is required. |
| P02 output | People Operations Specialist reviews the employee's response. Any disagreement with the joining date, unclear response, or exception is escalated to HR before confirmation. |
| P03 output | People Operations Specialist reviews the appointment letter against approved recruitment and employment information before release. |
| P04 output | People Operations Specialist confirms the correct appointment letter is used and reviews the returned signed document. Incorrect, missing, or inconsistent details require HR intervention. |
| P05 output | People Operations Specialist reviews the Fresh Graduate document checklist and confirms role-specific or mandatory items before collection continues. |
| P06 output | People Operations Specialist reviews the Experienced Employee document checklist and confirms employment-verification and reference requirements before collection continues. |
| P07 output | People Operations Specialist monitors outstanding documents and intervenes when documents are overdue, inconsistent, unreadable, or require an exception decision. |
| P08 output | People Operations Specialist validates employee data before synchronisation to HR/payroll and confirms the payroll information sent to Finance. |
| P09 output | People Operations Specialist assesses the device and access request and sends it for approval; the HR Manager approves equipment/access according to job title and work level. |
| P10 output | People Operations Specialist reviews the ID-card request and sends it to Admin. If employee name, phone number, job title, or another approved detail is incorrect, HR intervention is required before production. |


## Automation Boundary

AI is suitable for routine drafting, extraction, formatting, reminders, and structured handovers. Human accountability remains for changes to joining dates, employment terms, document exceptions, payroll validation, equipment/access approval, and identity-data corrections.


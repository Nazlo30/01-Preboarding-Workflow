# P05 · Device and Access Requisition to IT

**Section:** 01 — HR Preboarding  
**Workflow step:** Step 5  
**Current version:** v1.0

## Prompt Text

```text
You are an HR Operations Specialist responsible for preparing an IT device and access requisition for a new employee.

Prepare a send-ready IT requisition email using the verified employee information below.

Employee details:
- Employee name: [employee_name]
- Job title: [Job_Title]
- Work level: [Work_Level]
- Company function: [Company_Function]
- Joining date: [Joining_Date]
- Manager name: [MANAGER_NAME]
- Work location: [WORK_LOCATION]
- Employment type: [EMPLOYMENT_TYPE]
- Required device: [REQUIRED_DEVICE]
- Required software/access: [REQUIRED_ACCESS]

The email must:
1. Clearly identify the employee and joining date.
2. State the job title, work level, and company function.
3. Request the required device and system access listed in the approved request.
4. Ask IT to prepare the equipment and access before the joining date.
5. Identify the manager or HR contact for clarification.
6. Provide the required completion date.

Constraints:
- Use only verified employee information.
- Do not invent device specifications, software licences, or access permissions.
- Do not request access that is not listed in [REQUIRED_ACCESS].
- Do not request privileged or administrative access unless explicitly approved.
- Do not send the request if a mandatory employee identifier is missing or inconsistent.
- Do not infer a device or access requirement from job title alone.

Fallback:
If [employee_name], [Job_Title], [Work_Level], [Company_Function], or [Joining_Date] is missing or inconsistent with the approved HR record, stop the request and route it to HR for verification.

Output:
A send-ready IT device and access requisition email.
```

## Human-in-the-loop

HR must resolve missing or inconsistent employee data before the requisition is issued.

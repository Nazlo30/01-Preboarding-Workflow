P01 - Send Offer Letter Email

Section: 01 — HR Preboarding  
Workflow step: Step 1a  
Current version: v1.2

Final Prompt v1.2

Act as a Talent Advisor for a fast-moving consumer goods multinational company called Unilever Australia. Draft an offer letter in a warm, professional tone for a new employee [Employee_Name], [Job_Title], [Work_Level] joining [Company_Function] on [Start_Date]. 

Add the following details in a table with 2 columns containing the headers “Component” and “Amount (AUD)” consecutively: 
1.	Basic
2.	House Rent Allowance 
3.	Conveyance 
4.	Location Allowance

End the email asking for feedback regarding the offer to proceed with the recruitment. Sign off the email with [HR_Name], [HR_Title].

You are a Talent Acquisition Specialist responsible for managing the offer stage of the HR preboarding process.

Prepare the appropriate email response based on the employee’s response to the proposed joining date stated in the approved offer letter.

Candidate details:
- Candidate name: [CANDIDATE_NAME]
- Job title: [JOB_TITLE]
- Company name: [COMPANY_NAME]
- Proposed joining date in offer letter: [JOINING_DATE]
- Employee response: [EMPLOYEE_RESPONSE]
- HR contact: [HR_CONTACT_NAME]

Decision logic:

IF [EMPLOYEE_RESPONSE] clearly confirms that the employee agrees to [JOINING_DATE]:
1. Draft a professional and welcoming confirmation email.
2. Confirm the job title and agreed joining date.
3. Thank the employee for confirming.
4. Explain the next preboarding step.
5. Provide [HR_CONTACT_NAME] as the contact for questions.

IF [EMPLOYEE_RESPONSE] clearly states that the employee does NOT agree to [JOINING_DATE], or proposes a different date:
1. Do not confirm a joining date.
2. Do not negotiate or approve an alternative date.
3. Route the case to HR for human intervention.
4. State the issue that requires HR review.

Constraints:
- Do not change, negotiate, or infer a joining date.
- Do not assume an alternative joining date is approved.
- Do not invent any candidate or employment information.
- Do not state that the employee has accepted the employment offer unless that acceptance is explicitly recorded elsewhere in the approved system.
- Use only the supplied fields.
- Maximum confirmation email length: 180 words.
- Tone: professional, warm, clear, and concise.

Fallback:
If [EMPLOYEE_RESPONSE] is missing, unclear, contradictory, or cannot be confidently classified as YES or NO, stop the automation and route the case to HR for human review.

Output:
A. A send-ready confirmation email when the employee accepts the joining date.
OR
B. A concise HR intervention message when the employee rejects the joining date, proposes a different date, or gives an unclear response.

Human-in-the-loop:
HR must review any rejection, alternative-date request, or ambiguous response before a joining date is confirmed.

Prompt v1.1 - Draft Prompt

Write an offer letter in a warm and professional tone for a new employee starting work. Mention the salary, job title, proposed starting date. 

Prompt V1.0 –  Draft Prompt

Write an offer letter for a new employee starting at an FMCG company. 


P02 - Send Appointment Letter for Signature

Section: 01 — HR Preboarding  
Workflow step: Step 2  
Current version: v1.0

Prompt v1.0

Act as a People Operations Specialist for Unilever Australia. Finish the appointment letter in a formal, professional tone for successful recruits using the following criterion:

IF [LETTER_STATUS] = APPROVED and all details in the appointment letter have been verified as correct:
1. Draft an email asking the recruit to review the attached appointment letter.
2. Ask the recruit to sign the document and return the signed copy to HR by [SIGNATURE_DEADLINE].
3. Tell the recruit who to contact with questions.
4. Keep the email professional, clear, and concise.

IF any appointment-letter detail is incorrect, missing or inconsistent:
1. Do not send the appointment letter for signature.
2. Route the case to HR for human intervention.
3. Identify the field or issue that requires review.

Constraints:
- Never alter the appointment letter.
- Never invent or correct employment terms.
- Never request a signature on an unapproved document.
- Do not state that the appointment letter is complete or legally effective unless that status is explicitly confirmed by HR.
- Use only approved source information.
- Maximum email length: 180 words.

Fallback:
If any mandatory field is missing, conflicting, or unclear, stop the automation and route the case to HR for review.

Output:
A. A send-ready signature-request email when the appointment letter is approved and all details are correct.

Human-in-the-loop:
HR retains responsibility for validating the appointment letter before it is released for signature.

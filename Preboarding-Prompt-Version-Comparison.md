# Preboarding Prompt Version Comparison

This table compares all available versions of the 10 preboarding prompts using five test criteria:

1. Clear task definition
2. Business context
3. Tone controlled
4. Anti-hallucination instruction
5. Output format defined

Legend: ✅ = clearly meets criterion, ⚠️ = partially meets criterion, ❌ = does not meet criterion.

| Prompt | Version | Clear Task Definition | Business Context | Tone Controlled | Anti-Hallucination Instruction | Output Format Defined | Overall |
|---|---|---|---|---|---|---|---|
| **P01-A – Send Offer Letter** | v1.0 | ⚠️ Basic | ⚠️ Generic FMCG | ❌ | ❌ | ❌ | 🔴 **FAIL** |
| | v1.1 | ✅ Improved | ⚠️ Generic | ✅ | ❌ | ❌ | 🟠 **PARTIAL PASS** |
| | **v1.2 Final** | ✅ Strong | ✅ Unilever Australia | ✅ | ✅ | ✅ | 🟢 **PASS** |
| **P01-B – Manage Offer Response** | v1.0 | ⚠️ Basic follow-up | ❌ | ❌ | ❌ | ⚠️ Email implied | 🔴 **FAIL** |
| | v1.1 | ⚠️ Adds Yes/No decision | ❌ | ❌ | ❌ | ⚠️ Email implied | 🔴 **FAIL** |
| | **v1.2 Final** | ✅ Conditional workflow | ✅ HR offer stage | ✅ | ✅ | ✅ Email / HR routing | 🟢 **PASS** |
| **P02-A – Draft Appointment Letter** | v1.0 | ⚠️ Basic | ❌ | ❌ | ❌ | ⚠️ Letter + 150 words | 🔴 **FAIL** |
| | **v1.1 Final** | ✅ Strong | ✅ Unilever Australia / People Ops | ✅ | ⚠️ Fallback control | ✅ Email template | 🟢 **PASS*** |
| **P02-B – Appointment Signature** | v1.0 | ⚠️ Basic | ⚠️ HR implied | ✅ Professional | ❌ | ⚠️ Email implied | 🔴 **FAIL** |
| | v1.1 | ✅ Improved + deadline | ⚠️ HR implied | ✅ Professional | ⚠️ Incorrect-detail escalation | ⚠️ Email + 180 words | 🟠 **PARTIAL PASS** |
| | **v1.2 Final** | ✅ Strong conditional task | ✅ Unilever Australia / People Ops | ✅ | ✅ | ✅ Signature email / escalation | 🟢 **PASS** |
| **P03-A – New Graduate Documents** | v1.0 | ⚠️ Basic | ⚠️ Onboarding | ❌ | ❌ | ⚠️ Email implied | 🔴 **FAIL** |
| | v1.1 | ✅ Adds document list | ⚠️ Onboarding | ❌ | ❌ | ⚠️ Email + list | 🟠 **PARTIAL PASS** |
| | **v1.2 Final** | ✅ Strong | ✅ Unilever HR preboarding | ✅ | ✅ | ✅ Checklist + escalation | 🟢 **PASS** |
| **P03-B – Experienced Employee Documents** | v1.0 | ⚠️ Basic | ⚠️ Experienced hire | ❌ | ❌ | ⚠️ Email implied | 🔴 **FAIL** |
| | v1.1 | ✅ Adds document list | ⚠️ Experienced hire | ❌ | ❌ | ⚠️ Email + list | 🟠 **PARTIAL PASS** |
| | **v1.2 Final** | ✅ Strong | ✅ Unilever HR preboarding | ✅ | ✅ | ✅ Checklist + escalation | 🟢 **PASS** |
| **P03-C – Document Reminders** | v1.0 | ⚠️ Basic reminder | ⚠️ Onboarding | ❌ | ❌ | ⚠️ Reminder email | 🔴 **FAIL** |
| | **v1.1 Final** | ✅ Strong workflow | ✅ Unilever HR preboarding | ✅ | ✅ | ✅ List + reminder + escalation | 🟢 **PASS** |
| **P04 – Sync Employee Data** | v1.0 | ⚠️ Broad | ⚠️ Finance / Payroll | ❌ | ❌ | ❌ | 🔴 **FAIL** |
| | **v1.1 Final** | ✅ Strong validation workflow | ✅ HRS / Payroll / Finance | ⚠️ Professional context | ✅ | ✅ Four explicit outputs | 🟢 **PASS*** |
| **P05 – Device & Access Requisition** | v1.0 | ⚠️ Basic IT request | ⚠️ New joiner / IT | ❌ | ❌ | ⚠️ Email implied | 🔴 **FAIL** |
| | v1.1 | ✅ Adds work level + joining date | ⚠️ New joiner / IT | ❌ | ❌ | ⚠️ Email defined | 🟠 **PARTIAL PASS** |
| | **v1.2 Final** | ✅ Strong | ✅ HR → IT workflow | ⚠️ Professional implied | ✅ | ✅ Send-ready IT email | 🟢 **PASS*** |
| **P06 – ID Card Requisition** | v1.0 | ⚠️ Basic Admin request | ⚠️ New employee / Admin | ❌ | ❌ | ⚠️ Request implied | 🔴 **FAIL** |
| | v1.1 | ✅ Adds employee name + ID | ⚠️ New employee / Admin | ❌ | ❌ | ⚠️ Request defined | 🟠 **PARTIAL PASS** |
| | **v1.2 Final** | ✅ Strong validation workflow | ✅ HR → Admin workflow | ⚠️ Professional implied | ✅ | ✅ Approval / intervention | 🟢 **PASS*** |

## Version-Level Summary

| Version | Number of Prompts | General Result |
|---|---:|---|
| **v1.0** | 10 | 🔴 Mostly FAIL — basic task instructions with little control |
| **v1.1** | 10 | 🟠 Major improvement — more context, content and structure |
| **v1.2** | 7 | 🟢 Strongest — structured inputs, constraints, fallbacks and defined outputs |

## Overall Finding

The version progression shows a clear transition from basic generative prompting to governed HR workflow automation:

**v1.0 → Task definition**

Early prompts mainly tell the model what to do.

**v1.1 → Task + additional requirements**

The second iteration generally introduces important content, parameters, deadlines, document lists or tone controls.

**v1.2 → Controlled automation**

Where v1.2 exists, it generally introduces:

`structured inputs → decision rules → constraints → anti-hallucination rules → fallback → defined output → human review`

This makes v1.2 the strongest version where available.

### Notes

- P02-A, P03-C and P04 currently stop at **v1.1** in the repository; no v1.2 row has been invented.
- `* PASS with improvement opportunity` means the prompt meets the overall operational requirement, but at least one of the five criteria is only partially explicit.

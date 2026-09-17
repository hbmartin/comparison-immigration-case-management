# Immigration Case Management Software: Vendor Comparison

The biggest split in this market is between **immigration-native tools**, which are built around a forms engine and case types, and **general practice-management platforms** that bolt on immigration forms. Most firms end up choosing between a strong forms engine and strong firm operations, so decide early which one you can least afford to be weak.

**Scope:** Every column below can be scored from public sources — marketing and pricing pages, help centers, developer docs, trust centers and DPAs, release notes, app marketplaces, and app store listings. Nothing in the tables requires a demo, a trial, or a sales call. The questions that genuinely need hands-on time are parked in [Appendix A](#appendix-a-questions-that-need-a-demo) so they don't get quietly answered from a brochure. [Appendix B](#appendix-b-where-to-look) maps each kind of question to the source that settles it.

**How to use:** Add one row per vendor in each table. Fill cells with a score and a short note, and keep a source link plus the date you checked it.

| Mark | Meaning                                                      |
| ---- | ------------------------------------------------------------ |
| 5    | Documented in detail, with specifics you could hold them to  |
| 4    | Documented, but thin on specifics                            |
| 3    | Mentioned in marketing only                                  |
| 2    | Implied or available as a paid add-on                        |
| 1    | Explicitly not supported                                     |
| NS   | Not stated publicly                                          |

**`NS` is a finding, not a blank.** For a category a vendor competes on, silence usually means the answer is weak. Clusters of `NS` in security, API, pricing, and AI data handling are the ones that predict trouble; `NS` on a niche form is just noise.

### Contents

1. [Forms Engine](#1-forms-engine-usually-the-deciding-factor)
2. [Case Type Coverage](#2-case-type-coverage)
3. [Deadline and Status Tracking](#3-deadline-and-status-tracking)
4. [Workflow and Automation](#4-workflow-and-automation)
5. [Foreign-National Experience](#5-foreign-national-experience)
6. [Employer and HR Experience](#6-employer-and-hr-experience)
7. [Communications](#7-communications)
8. [Documents and Evidence](#8-documents-and-evidence)
9. [AI Capabilities](#9-ai-capabilities)
10. [AI Governance and Data Handling](#10-ai-governance-and-data-handling)
11. [Data Model and Extensibility](#11-data-model-and-extensibility)
12. [Reporting and Analytics](#12-reporting-and-analytics)
13. [Integrations and API](#13-integrations-and-api)
14. [Billing and Firm Operations](#14-billing-and-firm-operations)
15. [Security Posture](#15-security-posture)
16. [Data Governance and Portability](#16-data-governance-and-portability)
17. [Implementation and Onboarding](#17-implementation-and-onboarding)
18. [Cost and Vendor Risk](#18-cost-and-vendor-risk)

---

## At a Glance

One row per vendor, filled in before you score anything else. Every cell here is a yes/no lookup that takes a few minutes and tells you how much of the rest you'll actually be able to verify.

| Vendor        | Immigration-native or general | Target segment | Public pricing | Public API docs | Public trust center | Last checked |
| ------------- | ----------------------------- | -------------- | -------------- | --------------- | ------------------- | ------------ |
| _Vendor name_ | —                             | —              | —              | —               | —                   | —            |

- **Immigration-native or general:** Built around immigration case types and a forms engine, or a general practice-management platform with an immigration module. This single fact predicts most of the scores below.
- **Target segment:** Solo and small firm, mid-size, large firm, or corporate in-house. A tool sold to in-house teams often has the better employer portal and the weaker trust accounting.
- **Public pricing / API docs / trust center:** Three independent proxies for how much a vendor will tell you before you're in a sales cycle.

---

## 1. Forms Engine (usually the deciding factor)

| Vendor        | Form library coverage | Edition update cadence | Single-profile data reuse | Fee and supplemental handling | Filing output | Filed-version history |
| ------------- | --------------------- | ---------------------- | ------------------------- | ----------------------------- | ------------- | --------------------- |
| _Vendor name_ | —                     | —                      | —                         | —                             | —             | —                     |

- **Form library coverage:** USCIS, DOS (DS-160/260), DOL (ETA-9035 LCA, ETA-9089 PERM, ETA-9141 prevailing wage), and EOIR forms if you do removal defense. Most vendors publish a form list or a searchable library. Count the forms in your actual case mix rather than trusting the headline number.
- **Edition update cadence:** USCIS rejects outdated form editions. Public release notes are the evidence: look for dated entries naming specific form editions over the last year, and for a statement that in-progress cases migrate without re-entry. No public changelog is an `NS` here, and a meaningful one.
- **Single-profile data reuse:** Enter data once and have it populate every form in a bundle (I-130/I-485/I-765/I-131), and carry across derivatives, extensions, and amendments. Help-center articles about "profiles," "smart forms," or "data reuse" reveal whether data lives in a person record or is re-keyed per form. This drives most of your paralegal time savings.
- **Fee and supplemental handling:** Whether the tool calculates current filing fees and attaches G-28, G-1145, and I-907 automatically. Fee schedules change — substantially in 2024 — so look for a dated commitment to tracking the current schedule, not just a fee calculator screenshot.
- **Filing output:** PDF fidelity (barcodes intact) and signature handling. Check whether it supports USCIS online filing or only generates PDFs for mailing, and whether it works with USCIS organizational accounts for H-1B registration and shared online filing. Online filing coverage is form-specific and changes, so get the list.
- **Filed-version history:** Whether the docs describe a locked snapshot of what was actually filed, dated and separate from the current editable data. This is the line between a records system and a PDF generator.

## 2. Case Type Coverage

A generic platform can technically hold an immigration matter while making staff fight it daily. What you're checking here is whether your case types arrive as first-class, preconfigured things or as empty matters you assemble yourself.

| Vendor        | Employment-based | Family and humanitarian | Consular processing | Removal and EOIR | Naturalization | Case-type templates |
| ------------- | ---------------- | ----------------------- | ------------------- | ---------------- | -------------- | ------------------- |
| _Vendor name_ | —                | —                       | —                   | —                | —              | —                   |

- **Employment-based:** Named coverage for H-1B (cap and cap-exempt), L-1A/L-1B and blanket L, O-1, TN, E-1/E-2/E-3, H-1B1, PERM, and I-140 across EB-1/EB-2/EB-3 including NIW. Extensions, amendments, transfers, and AC21 portability should appear as their own case types, not be implied by "H-1B."
- **Family and humanitarian:** I-130, adjustment of status, K-1, I-751, asylum, VAWA, U and T visas, TPS. Score this low without apology if you're a business-immigration practice — just don't let a vendor's breadth here paper over thinness in the column that matters to you.
- **Consular processing:** DS-160 and DS-260 support, NVC document handling, and interview tracking. Frequently the weakest area in otherwise strong platforms.
- **Removal and EOIR:** EOIR-28, EOIR-42A/42B, ECAS filing, master and individual hearing tracking, bond. Drop this column entirely if you don't do removal work.
- **Naturalization:** N-400, N-600, and any eligibility or physical-presence calculators.
- **Case-type templates:** Whether each case type ships as a configured template — checklist, forms, tasks, and deadlines together — or as a blank matter. Help-center screenshots usually settle this faster than the marketing page.

## 3. Deadline and Status Tracking

| Vendor        | Case status sync | Priority dates | Expiration tracking | Response deadlines | Calendar sync | Seasonal volume |
| ------------- | ---------------- | -------------- | ------------------- | ------------------ | ------------- | --------------- |
| _Vendor name_ | —                | —              | —                   | —                  | —             | —               |

- **Case status sync:** Does it pull status automatically from USCIS by receipt number, or rely on scraping or manual checks? Ask for the stated mechanism — an official API, organizational accounts, or scraping. Scraping breaks, quietly, at the worst times.
- **Priority dates:** It should track priority dates against the monthly Visa Bulletin and alert you when a date becomes current. Check that it handles both the Final Action Dates and Dates for Filing charts, and follows USCIS's monthly choice between them.
- **Expiration tracking:** I-94, EAD, visa stamps, passports, H-1B six-year max-out (with recapture), LCA validity, and PERM recruitment and prevailing-wage validity windows.
- **Response deadlines:** RFE/NOID deadlines, EOIR hearing dates, and I-751/I-829 filing windows.
- **Calendar sync:** Two-way Outlook and Google Calendar sync, verifiable on the integrations page and in the vendor's Microsoft AppSource or Google Workspace Marketplace listing.
- **Seasonal volume:** Bulk workflows for H-1B cap season — bulk registration, bulk questionnaire sends, lottery-result intake, and mass status updates.

## 4. Workflow and Automation

Score this against a real scenario rather than a feature list. The reference case: *an H-1B is opened for an existing employee of an existing corporate client.* From public documentation, how much of the following is automated versus clicked — send the questionnaire, request documents, assign paralegal tasks, calculate deadlines, generate drafts, route attorney review, collect signatures, file, notify stakeholders, and schedule expiration reminders?

| Vendor        | Workflow templates | Triggers and automation | Conditional logic | Date and deadline rules | Review routing | Bulk actions |
| ------------- | ------------------ | ----------------------- | ----------------- | ----------------------- | -------------- | ------------ |
| _Vendor name_ | —                  | —                       | —                 | —                       | —              | —            |

- **Workflow templates:** A published library of per-case-type workflows, and whether you can edit them or only use them as shipped.
- **Triggers and automation:** What events can start an automation (case opened, status changed, document received, date reached) and what actions it can take. A vendor's Zapier listing enumerates its published triggers and actions, which is often more specific than its own marketing page.
- **Conditional logic:** Whether workflows branch on case data — different tasks for a change of status versus a consular notification, or for a cap-exempt employer. Look for "if/then," "branching," or "conditional" in the automation docs.
- **Date and deadline rules:** Deadlines calculated from case events (receipt date, RFE issue date, I-94 expiry) rather than typed in by hand, and recalculated when the anchor date changes.
- **Review routing:** Paralegal-to-attorney review handoffs as a documented state, with assignment and approval recorded — not a task named "attorney review."
- **Bulk actions:** Bulk status changes, bulk task assignment, and bulk sends across a filtered set of matters.

## 5. Foreign-National Experience

Evaluate this separately from the employer experience below. The two audiences want opposite things, and most platforms are clearly better at one.

| Vendor        | Portal and mobile | Questionnaire capability | Prepopulation | Document collection status | Language coverage |
| ------------- | ----------------- | ------------------------ | ------------- | -------------------------- | ----------------- |
| _Vendor name_ | —                 | —                        | —             | —                          | —                 |

- **Portal and mobile:** A web portal plus native iOS/Android apps. App Store and Google Play listings independently confirm the apps exist, when they were last updated, which languages they ship, and what users say. A client app with no update in a year tells you where the roadmap isn't.
- **Questionnaire capability:** Conditional questions and skip logic, save-and-resume, and questionnaires that differ by case type. Immigration intake is unusually repetitive, so branching matters more here than in most legal software.
- **Prepopulation:** Whether a returning client sees their own prior answers already filled. Clients should not re-enter passport details, addresses, employment history, or corporate information the firm already holds. Language about reusable beneficiary profiles is the signal; "send a new questionnaire" is the anti-signal.
- **Document collection status:** Whether checklists distinguish **requested**, **received**, **reviewed**, and **accepted** as separate states, whether checklists change based on answers, and whether expiring documents (passports, I-94s) are tracked and re-requested. Help-center screenshots show the actual status labels.
- **Language coverage:** The published list of supported languages, and whether it covers questionnaires and generated correspondence or only the interface. App store listings also enumerate supported languages, independently of marketing claims.

## 6. Employer and HR Experience

| Vendor        | HR dashboard | Self-service case initiation | Scoped access | Employer reporting | Multi-entity support | I-9 and LCA compliance |
| ------------- | ------------ | ---------------------------- | ------------- | ------------------ | -------------------- | ---------------------- |
| _Vendor name_ | —            | —                            | —             | —                  | —                    | —                      |

- **HR dashboard:** An employee roster showing visa types, expiration dates, case status, and outstanding actions in one view. Essential for business immigration, and the single most common gap in family-immigration-first products.
- **Self-service case initiation:** Whether HR can start a case, upload documents, and approve drafts without emailing the firm.
- **Scoped access:** Whether an HR user can be limited to a subset of employees, entities, or locations, and whether privileged work product and unrelated matters stay hidden. Look for a published permissions matrix, not a sentence about "role-based access."
- **Employer reporting:** Headcount by visa type, upcoming expirations, case pipeline, and spend — exportable by the client themselves.
- **Multi-entity support:** Parent/subsidiary hierarchies, multiple worksites, and multiple contacts per corporate account.
- **I-9 and LCA compliance:** I-9 and E-Verify support, LCA public access file tracking, and the Form I-129 Part 6 export-control attestation. These are often separate products or paid add-ons, so check whether they're included.

## 7. Communications

Efficiency differences here are larger than they look on a feature list.

| Vendor        | Email capture | Inbound reply handling | SMS and messaging | Templates and bulk send | Automated reminders | Internal vs client-visible |
| ------------- | ------------- | ---------------------- | ----------------- | ----------------------- | ------------------- | -------------------------- |
| _Vendor name_ | —             | —                      | —                 | —                       | —                   | —                          |

- **Email capture:** A native Outlook or Gmail integration that files messages to the right matter, versus a BCC drop address versus manual copy-paste. The marketplace listing tells you which.
- **Inbound reply handling:** What the docs say happens when a client replies to an ordinary email instead of using the portal. Many portal-centric products handle this badly, and clients do it constantly.
- **SMS and messaging:** SMS and WhatsApp support, whether messages are logged to the case, and whether volume is included or metered.
- **Templates and bulk send:** Merge-field templates and bulk sends to a filtered group — every H-1B expiring within 120 days, for example.
- **Automated reminders:** Documented reminder sequences for missing documents and unfinished questionnaires, with per-contact frequency and channel preferences.
- **Internal vs client-visible:** A clear separation between internal notes and client-visible messages, with one chronological history per matter covering email, SMS, portal messages, and calls.

## 8. Documents and Evidence

| Vendor        | Exhibit assembly | Case-type checklists | Document generation | Conditional templates | E-signature | OCR and extraction |
| ------------- | ---------------- | -------------------- | ------------------- | --------------------- | ----------- | ------------------ |
| _Vendor name_ | —                | —                    | —                   | —                     | —           | —                  |

- **Exhibit assembly:** Auto-indexing, tabs, bookmarks, and file compression to meet USCIS upload and mailing limits.
- **Case-type checklists:** Checklists per case type, plus translation certification tracking.
- **Document generation:** Beyond government forms — engagement letters, employer support letters, petition letters, declarations, filing covers, and RFE responses generated from matter data. Look for a published Word/PDF template library, and for whether templates are firm-editable.
- **Conditional templates:** Conditional clauses and repeating sections, not simple `{{first_name}}` mail merge. Documentation mentioning if/then logic or repeating blocks is the tell; a screenshot of merge fields is not.
- **E-signature:** Native e-sign or an integration (DocuSign, Adobe Acrobat Sign, Dropbox Sign), and whether envelopes are included or billed separately. The partner's own app directory confirms whether the integration is real and maintained.
- **OCR and extraction:** Passport MRZ scanning, I-94 and prior-petition extraction, and — the part that matters — whether extracted values land in structured fields or just sit in an attachment.

## 9. AI Capabilities

Don't score a product highly because the vendor says "AI." Score each capability separately; a page that says "AI-powered" without naming one is `NS` across this entire row.

| Vendor        | Data extraction | Summarization | Drafting | Semantic search | Classification and gap detection | RFE analysis |
| ------------- | --------------- | ------------- | -------- | --------------- | -------------------------------- | ------------ |
| _Vendor name_ | —               | —             | —        | —               | —                                | —            |

- **Data extraction:** Structured extraction from passports, I-94s, prior petitions, resumes, and degree evaluations into fields the case actually uses.
- **Summarization:** Summaries of long case histories and correspondence threads.
- **Drafting:** Support letters, RFE responses, and client emails. Check whether the published examples are immigration-specific or generic legal boilerplate with a visa word swapped in.
- **Semantic search:** Search across case files and documents, and whether results carry citations back to the source document and page.
- **Classification and gap detection:** Automatic document classification into checklist slots, and missing-information detection against a case type's requirements.
- **RFE analysis:** Parsing an RFE into its discrete requests and mapping each to existing evidence. The most frequently claimed and least frequently specified capability in this market.

## 10. AI Governance and Data Handling

| Vendor        | Training on customer data | Model and subprocessor disclosure | Prompt and document retention | Human review and audit trail | Tenant and matter isolation | Admin controls |
| ------------- | ------------------------- | --------------------------------- | ----------------------------- | ---------------------------- | --------------------------- | -------------- |
| _Vendor name_ | —                         | —                                 | —                             | —                            | —                           | —              |

- **Training on customer data:** A written commitment in the terms or DPA that your data is not used to train models — not a reassuring sentence on a marketing page. Check that it binds subprocessor model providers too, not just the vendor.
- **Model and subprocessor disclosure:** Which models and providers process your data, named in a published subprocessor list. "Enterprise-grade AI" is `NS`.
- **Prompt and document retention:** How long prompts, outputs, and uploaded documents are retained by the vendor and by the model provider. Zero-retention arrangements should be stated, not assumed.
- **Human review and audit trail:** Whether AI output is always a draft pending human approval, and whether AI-generated content is attributed and traceable in the audit log back to its source.
- **Tenant and matter isolation:** An explicit statement that AI retrieval cannot cross client or matter boundaries. This is a conflicts question and, for asylum material under 8 CFR 208.6, a confidentiality one.
- **Admin controls:** Whether AI features can be disabled per firm, per user, per matter, or per client. Firms with asylum, government, or security-cleared clients usually need this.

## 11. Data Model and Extensibility

Ideally a person's passport number, status, employer, position, worksite, addresses, family relationships, and immigration history exist once, as structured reusable data. Otherwise the same fact ends up copied across:

```
I-129 → questionnaire → contact record → custom field → I-140 → Word template
```

…and those copies inevitably disagree. Help-center documentation is unusually revealing here — the way articles talk about contacts, profiles, and beneficiaries shows you the underlying model.

| Vendor        | Reusable person records | Employer hierarchy | Family relationships | Immigration history | Custom fields and objects | Bulk edit and import |
| ------------- | ----------------------- | ------------------ | -------------------- | ------------------- | ------------------------- | -------------------- |
| _Vendor name_ | —                       | —                  | —                    | —                   | —                         | —                    |

- **Reusable person records:** Whether a person exists once and is linked to many matters, with passport, status, employer, position, worksite, and addresses as structured fields — or whether every matter re-collects them.
- **Employer hierarchy:** Corporate accounts with parent/subsidiary structure, multiple worksites, and multiple contacts per account, plus multiple concurrent matters per employer.
- **Family relationships:** Spouse and dependent links that actually drive derivative filings, rather than a free-text "relationship" field.
- **Immigration history:** Prior petitions, approvals, entries, and status changes as dated structured records you can report on.
- **Custom fields and objects:** Which record types accept custom fields, whether you can define new object types, whether statuses are configurable, and whether field-level permissions exist.
- **Bulk edit and import:** Bulk editing, CSV import, and published import templates. The existence of documented import templates tells you a great deal about how structured the model underneath really is.

## 12. Reporting and Analytics

Don't ask whether it "has reports." Take the questions your managing attorney or operations lead actually asks and check whether the published report list could answer them:

> How many cases are waiting on the client versus waiting on our firm? Which employees have immigration expirations in the next 120 days? What's our median time from case opening to questionnaire completion? Which cases have had no activity for 14 days? How long do attorneys take to review drafts after a paralegal submits them? What percentage of clients complete questionnaires without staff intervention? What is the average number of client follow-ups per matter type?

A vendor that publishes only dashboard screenshots is a 3 at best, however good the screenshots look.

| Vendor        | Standard report library | Custom report builder | Cross-object reporting | Dashboards | Scheduled delivery and export | BI and warehouse access |
| ------------- | ----------------------- | --------------------- | ---------------------- | ---------- | ----------------------------- | ----------------------- |
| _Vendor name_ | —                       | —                     | —                      | —          | —                             | —                       |

- **Standard report library:** A published list of canned reports. Count how many of the questions above they'd answer as shipped.
- **Custom report builder:** Whether you can build reports with your own filters and groupings, without buying vendor services each time.
- **Cross-object reporting:** Whether a report can span matters, people, employers, tasks, and communications, or only one object at a time. This is the line between analytics and a few canned dashboards.
- **Dashboards:** Role-based dashboards for attorneys, paralegals, and managers, plus pipeline, turnaround times, approval/RFE rates, and revenue by case type.
- **Scheduled delivery and export:** Scheduled email delivery, CSV/Excel export, and whether exports are row-limited.
- **BI and warehouse access:** Read-only database access, a warehouse sync, or a documented bulk-export API for Power BI, Tableau, or Snowflake. Also the escape hatch when the built-in reporting can't answer something.

## 13. Integrations and API

Classify every integration as **native**, **Zapier-mediated**, or **"we have an API, build it yourself."** Vendor integration pages routinely list all three together as if they were equivalent. Even if you don't need the API today, this section determines how trapped you are later.

| Vendor        | Email and calendar | E-signature and payments | Accounting and storage | HRIS and identity | Public API | Webhooks and sandbox |
| ------------- | ------------------ | ------------------------ | ---------------------- | ----------------- | ---------- | -------------------- |
| _Vendor name_ | —                  | —                        | —                      | —                 | —          | —                    |

- **Email and calendar:** Microsoft 365 and Google Workspace with two-way calendar sync. A live listing in Microsoft AppSource or the Google Workspace Marketplace confirms a real, maintained app.
- **E-signature and payments:** DocuSign, Adobe Acrobat Sign, or Dropbox Sign; LawPay, Stripe, or Gravity Legal. Partner app directories confirm these independently of the vendor's own claims.
- **Accounting and storage:** QuickBooks or Xero; SharePoint, OneDrive, Google Drive, NetDocuments, or iManage.
- **HRIS and identity:** Workday, SuccessFactors, BambooHR, UKG, or a unified HRIS layer; Okta or Entra ID for SSO. A listing in the Okta Integration Network independently confirms SAML support the security page may only gesture at.
- **Public API:** Publicly readable REST or GraphQL documentation, with auth model, object coverage, and rate limits stated. "API available on request" is `NS`, and usually means a services engagement.
- **Webhooks and sandbox:** Documented webhook events, a sandbox or test tenant, service accounts for automation, and a documented bulk export.

## 14. Billing and Firm Operations

| Vendor        | Billing models | Trust accounting | Payment processing | Front office | Time tracking |
| ------------- | -------------- | ---------------- | ------------------ | ------------ | ------------- |
| _Vendor name_ | —              | —                | —                  | —            | —             |

- **Billing models:** Flat-fee and milestone billing, payment plans, and hourly billing for litigation work. For business immigration, check split billing between employer and beneficiary — some H-1B fees cannot lawfully be passed to the employee, so the split has to be modeled, not improvised.
- **Trust accounting:** Full IOLTA compliance, including three-way reconciliation and correct handling of government filing fees as client funds.
- **Payment processing:** Online payments and ACH, and whether the processor is bundled or your choice.
- **Front office:** Lead intake, consult scheduling, conflict checks.
- **Time tracking:** Timers and mobile entry, and whether flat-fee matters can still capture time for profitability reporting.

## 15. Security Posture

You'll hold A-numbers, SSNs, passports, birth certificates, financial records, and asylum material, which has heightened confidentiality under 8 CFR 208.6. "We're HIPAA compliant" and "bank-level security" are not answers to any of the following.

| Vendor        | Certifications | Encryption | Authentication and SSO | Access control | Audit logs | Availability and DR |
| ------------- | -------------- | ---------- | ---------------------- | -------------- | ---------- | ------------------- |
| _Vendor name_ | —              | —          | —                      | —              | —          | —                   |

- **Certifications:** SOC 2 Type II, ISO 27001, and a penetration-test summary. A trust center (Vanta, Drata, SafeBase, Conveyor) with a request-under-NDA flow is the strongest public signal. Check that the report is **Type II**, not Type I, and that its period is current.
- **Encryption:** Encryption in transit and at rest with algorithms and key management described, plus any customer-managed key option.
- **Authentication and SSO:** MFA for all users, SAML 2.0 SSO, SCIM provisioning, and session policy. Check which plan tier SSO requires — it's frequently gated behind the most expensive one.
- **Access control:** Role-based access, matter-level and client-level restrictions, ethical walls, and field-level permissions. A published permissions matrix scores 5; a paragraph scores 3.
- **Audit logs:** What is logged, whether admins can view and export it themselves, and how long it's retained.
- **Availability and DR:** A public status page with incident history, a published uptime commitment, backup frequency, and stated RPO/RTO.

## 16. Data Governance and Portability

| Vendor        | Hosting and residency | Subprocessors | Retention and deletion | Export and portability | Breach commitments | Ethics fit |
| ------------- | --------------------- | ------------- | ---------------------- | ---------------------- | ------------------ | ---------- |
| _Vendor name_ | —                     | —             | —                      | —                      | —                  | —          |

- **Hosting and residency:** Cloud provider and region, and whether data can be pinned to a specific country if a client requires it.
- **Subprocessors:** A published, dated subprocessor list with a change-notification commitment. An unpublished list is `NS` and a negative — it's the only way to see who else touches your clients' documents.
- **Retention and deletion:** Retention periods, deletion on request, and what happens to backups after deletion. Also employee and subprocessor access policy.
- **Export and portability:** Whether you can export structured case data — not just PDFs — and whether the format is documented. Ask for a sample export before signing. This is the most commonly skipped check and the most painful one later.
- **Breach commitments:** Notification timelines in the DPA or terms, stated in hours or days rather than "promptly."
- **Ethics fit:** Check the vendor against your state bar's cloud-computing guidance and ABA Formal Opinion 512 on generative AI, and confirm how asylum material under 8 CFR 208.6 is handled.

## 17. Implementation and Onboarding

| Vendor        | Migration support | Documented importers | Training resources | Self-service configuration | Published timelines | Support model |
| ------------- | ----------------- | -------------------- | ------------------ | -------------------------- | ------------------- | ------------- |
| _Vendor name_ | —                 | —                    | —                  | —                          | —                   | —             |

- **Migration support:** Whether migration is included, separately priced, or DIY, and which source systems have named migration paths (INSZoom, LawLogix, Clio, MyCase, spreadsheets).
- **Documented importers:** Published import templates and field mappings. Their existence — and how granular they are — is a good independent read on how structured the data model is.
- **Training resources:** A public help center, video library, certification program, and user community. Depth here predicts how much your staff can solve without opening a ticket.
- **Self-service configuration:** Whether templates, workflows, questionnaires, custom fields, and statuses are admin-configurable, or require a paid services engagement each time.
- **Published timelines:** Any stated typical go-live time. Rarely published, so `NS` is common here; a vendor that does publish one is worth taking seriously.
- **Support model:** Support channels, hours and time zones, named CSM, and whether a published SLA exists at your tier.

## 18. Cost and Vendor Risk

| Vendor        | Pricing model | Pricing transparency | Contract terms | Roadmap and release cadence | Vendor stability | Reference base |
| ------------- | ------------- | -------------------- | -------------- | --------------------------- | ---------------- | -------------- |
| _Vendor name_ | —             | —                    | —              | —                           | —                | —              |

- **Pricing model:** Per user, per case, or per form. Itemize what's charged separately — portals, e-filing, AI, SMS, e-sign envelopes, storage, extra entities, sandbox.
- **Pricing transparency:** Real published numbers, a published range, or "contact sales." How much a vendor will say before a sales call is a fair proxy for how the rest of the relationship goes.
- **Contract terms:** Minimum term, seat minimums, renewal escalators, onboarding fees, and termination and export terms — usually findable in a public MSA or terms page.
- **Roadmap and release cadence:** A public changelog with dated entries across the last twelve months, and a public roadmap if one exists. Two quiet quarters is a signal, especially after an acquisition.
- **Vendor stability:** Ownership, funding history, acquisitions, and headcount trend. This space has consolidated significantly, so confirm who owns the product today and whether it's still being invested in rather than harvested.
- **Reference base:** Named customers, case studies, and third-party review volume and recency. Recent reviews from firms your size and practice mix are worth more than a logo wall.

---

## Appendix A. Questions That Need a Demo

These are deliberately **not** in the tables above, because no marketing page can answer them honestly. Keep them as your demo script, and don't let a vendor answer them from a slide.

- **The scenario test.** "An H-1B case is opened for an existing employee of an existing corporate client." Count the manual actions needed to send the questionnaire, request documents, assign paralegal tasks, calculate deadlines, generate drafts, route attorney review, collect signatures, file, notify stakeholders, and schedule expiration reminders. Repeat for a PERM and an RFE response.
- **Where the data actually lives.** Have them show you one beneficiary's passport number everywhere it appears, then change it once. Whether the change propagates is the entire test.
- **Form fidelity.** Print a completed I-129 bundle and inspect barcodes, page breaks, and signature blocks.
- **Prepopulation in practice.** Open a second matter for the same beneficiary and see what's already filled before anyone types anything.
- **AI accuracy.** Run their extraction and drafting against five of your own closed files and grade the output yourself.
- **Inbound email behavior.** Reply to a portal notification from an ordinary email client and find out where it lands.
- **HR scoping.** Log in as an HR user and try to reach an employee or a document they shouldn't see.
- **Reporting.** Hand them the operational questions from section 12 and have them build the reports live.
- **Import quality.** Give them a real export from your current system and have them import it, then check what got dropped.
- **Support under load.** Ask for March and April response-time data, and for references you select from their customer list rather than ones they pick.

## Appendix B. Where to Look

| Source                                                       | What it settles                                                       |
| ------------------------------------------------------------ | --------------------------------------------------------------------- |
| Pricing page                                                 | Pricing model, tiers, which features are gated or add-ons             |
| Help center / knowledge base                                 | Data model, permissions, questionnaires, checklists, statuses         |
| Release notes / changelog                                    | Form edition cadence, release velocity, whether the product is alive  |
| Developer docs                                               | API existence and shape, auth, object coverage, webhooks, rate limits |
| Trust center / security page                                 | SOC 2 Type II, ISO 27001, encryption, SSO, pen tests                  |
| DPA, terms, and subprocessor list                            | Model providers, AI training terms, retention, residency, breach notice |
| App marketplaces (AppSource, Google Workspace, DocuSign, Zapier, Okta) | Which integrations are real, native, and maintained          |
| App Store / Google Play                                      | Mobile apps, update recency, supported languages, user sentiment      |
| Status page                                                  | Uptime history and incident transparency                              |
| G2 / Capterra                                                | Review recency and volume, segmented by firm size                     |
| LinkedIn / Crunchbase / trade press                          | Ownership, funding, headcount trend, acquisitions                     |

Record the date you checked each source. Form editions, fee schedules, pricing, integration lists, and subprocessor lists all change, and a comparison built from undated evidence goes stale without ever looking wrong.

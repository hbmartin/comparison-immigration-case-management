# Ranked recommendations

Interview-weighted ranking of vendors in [README.md](README.md) for this firm. Research in the comparison tables is dated **2026-09-17**. Scores there are conservative and search-extracted; treat every cell as a demo question, not a verdict.

## Buyer profile

Small immigration **law firm**, **4–15 people**, **greenfield** (nothing structured today), **Google Workspace**. Billing stays where it is (QuickBooks, LawPay, or similar). Success this quarter: staff **live in a CMS within weeks** — intake, forms, e-file, documents.

Case mix is **~70%+ employment**, but the firm’s identity is **O-1 / EB-1 / NIW**, with **H-1B cap as a fire drill**, not the product. Family is the minority and still a hard requirement: **I-130 / I-485 / I-765 / I-131 from one profile**. Petitioners are a **mix of companies and individuals**; both have to feel native.

The firm will **build a stack**. Two products is fine. The second product must **prefill or round-trip government forms**, not only Word letters, and should **learn voice from past winning petitions**. Status updates should live **inside the CMS** (receipt sync, then email/SMS). SMS is wanted, not a v1 killer. Employer portal is nice-to-have. Security bar for v1 is **MFA + a vendor the firm can live with**; a startup is acceptable if it is clearly better on premium packets.

**Hard gates for the system of record:** it must be the case/forms CMS, and it must **e-file to USCIS** (the firm still mails a lot of PDFs). Cap season in the next 90 days means **people, questionnaires, and docs in the system**, not a lottery module.

Those gates, not generic feature richness, produce the order below.

## How the ranking is weighted

| Weight | What it does |
| --- | --- |
| **Disqualify as CMS** | Not a system of record; no credible USCIS e-file; cannot do a family AOS bundle; implementation is a sales-led project, not weeks |
| **Highest** | Forms engine + one-profile reuse; USCIS e-file; O-1/EB-1/NIW letters, exhibits, RFEs; drafting that fills forms; Google/Gmail; go-live speed |
| **High** | Receipt sync inside the CMS; questionnaires + document upload; firm-voice learning; paralegal prepares / attorney revises |
| **Medium** | SMS; H-1B as structured data not Excel; company + individual intake; exhibit indexes; Visa Bulletin (family AOS + some NIW) |
| **Low / ignore for v1** | Billing, trust, I-9, removal, HR portal, DOL FLAG, DS-160, SOC 2 bake-off |

Point solutions are ranked as **add-ons**, not as CMS replacements.

## Ranked fits

### 1. Docketwise + Parley — best stack

This is the only pairing that hits the **CMS gates** and the **drafting gates** without pretending one product does both well.

**Docketwise as system of record.** Public pricing, help center, admin-built matter types, **native Gmail add-on**, two-way Google Calendar, **USCIS / DOL FLAG / DOS CEAC e-file**, strongest public **forms library** in the comparison, **one-intake form bundles** (the AOS package that was non-negotiable), **receipt-number sync**, **two-way SMS**, and **Visa Bulletin / priority-date tracking**. That last piece matters for family AOS and for NIW even if EB-1 is current. Implementation matches “live in weeks.” Billing weakness is irrelevant.

**Parley as the O-1 / EB-1 / NIW layer.** Matches how the firm works: paralegals assemble from prior matter, attorney revises. It extracts passport / I-94 / I-797 into **I-129 / I-140 / I-907 / G-28 / I-539 / I-765**, drafts in **firm voice from prior cases**, parses RFEs and maps evidence, and builds exhibit packets. Named customers in the report are employment-premium firms, not consumer filers.

**Why this is #1 rather than a single vendor.** Docketwise’s own AI is extraction + rewrite. It does **not** draft petition letters or RFEs. Parley is **not** a CMS, has **no e-file**, and is employment-first on family. Split the jobs on purpose: Docketwise owns the matter, family bundles, Google, status, SMS, e-file. Parley owns the premium petition.

**The integration risk not to paper over.** The report does **not** document a native Docketwise connector. Parley imports from Drive/OneDrive/Dropbox and exports PDF packets. The bar was “round-trip government forms,” which Parley does **inside Parley**. The unproven step is: filled forms + packet → Docketwise matter → Docketwise e-file, without re-keying. That is the first demo script, not a reason to pick a weaker CMS.

**Skip if:** the firm will only run one login forever, or needs a certified two-way forms API on day one.

### 2. Docketwise + CaseBlink — same CMS, narrower and sharper add-on

Same CMS reasons as #1. CaseBlink is the better **identity match** if almost all premium work is **O-1A/O-1B and EB-1A/B/C**: exhibit organization, Studio voice, I-129 named, packet assembly.

It is **#2 rather than #1** because the public form set is narrower than Parley’s, family is absent (so Docketwise must own 100% of AOS), RFE is “draft a response” not “parse requests and map evidence,” and there is **no** Drive import, API, or Gmail bridge in the report. For a Google-first firm that also files NIW and H-1B, Parley covers more of the docket.

**Pick this over Parley if** a CaseBlink demo on a real last EB-1A packet is clearly more usable than Parley, and NIW/H-1B letters can stay in Word for a while.

### 3. Docketwise alone, Parley/CaseBlink in month two — best if the quarter is the constraint

If “staff live in the CMS in weeks” is the only outcome that matters, **buy Docketwise first** and do not wait to pick the AI layer.

Intake, Smart Forms, e-file, Gmail, status, SMS, and AOS bundles land immediately. Letter drafting and exhibit indexes will still hurt — that is documented in the comparison (drafting **2**, RFE **NS**, exhibit index **NS**). Add Parley or CaseBlink once matters are no longer in spreadsheets.

This is the lowest-risk path that still matches every **CMS** gate. It is #3 not #1 because the second product was required to touch forms and learn voice. This delays a stated requirement; it does not drop it.

### 4. eIMMIGRATION + Parley — strongest alternative CMS stack

eIMMIGRATION is the other small-firm CMS that is actually **immigration-native, publicly priced, self-serve, and USCIS-e-file capable**. It beats Docketwise on **packet assembly** (merged PDF with contents), **Extractor AI**, **120+ prebuilt processes**, and **Google Drive / Box / Dropbox / OneDrive** (Docketwise has **no** cloud-storage connector in the report). Family coverage is via a large USCIS library rather than named AOS bundles — verify I-130/485/765/131 reuse in the demo.

It ranks under Docketwise because of **this firm’s** priorities, not because it is a worse product in general:

- Status sync is weaker and the mechanism is unstated (**3** vs Docketwise **4**).
- **No SMS** in the report; status **and** texts were wanted inside the CMS.
- E-file is a **Chrome extension**, not documented native e-file. Fine for many firms; org-account online filing is real work here.
- Priority dates: nightly Visa Bulletin, **final action only** — Docketwise tracks both charts.
- Gmail is listed, not a verified Workspace add-on with the same weight as Docketwise’s native add-on.
- Drafting “4” is **Visalaw GEN**, which does **not** fill USCIS forms. “Just Word letters” was already rejected. Parley (or similar) would still sit on top, which is three moving parts unless Visalaw is dropped.

**Pick this over Docketwise** if the demo shows better AOS packet PDFs, Drive as the document spine, and email-only status alerts are acceptable for 90 days.

### 5. eIMMIGRATION + Visalaw.ai (their own GEN partnership) — cleanest *documented* two-product stack, wrong drafting job

This is the only CMS + AI pair in the report that is a **named partnership**. Implementation and one throat to choke are better. Visalaw is strong at letters, briefs, cited research, and summarization, with a written no-train / zero-retention stance.

It is #5 because the drafting layer was required to **prefill government forms**. Visalaw’s forms-engine scores are **1** across the board. eIMMIGRATION Extractor can land passport data in fields; Visalaw still will not round-trip I-129/I-140. For an O-1/EB-1 firm whose paralegals already assemble from old samples, Parley/CaseBlink are the better second product.

### 6. Legal Bridge — highest-ceiling single product, weakest evidence

On **marketing shape** this is the firm: AI-first CMS, **H-1B / O-1 / EB-1 / NIW**, family categories named, claimed **USCIS + DOL FLAG + DOS** e-file, exhibit lists, firm-style drafting, Gmail/Outlook, client portal, missing-doc alerts.

It is not top-three because the comparison cannot verify the non-negotiables: form library is **2** (DS-160 and LCA named, no count), e-file is a claim (**3**), AOS one-profile bundles are not documented, receipt sync is **2**, SMS is absent, help center / support hours / SLA are **NS**, public pricing is not real numbers. Founded 2023, ~80–100 firms claimed.

**Keep it on the demo list** because a startup CMS was allowed if O-1/EB-1 packets are clearly better. Promote it only if a hands-on trial files a real I-140 and a real I-130/485 bundle and shows e-file, not slides.

### 7. Imagility — best “petition machine,” fails the CMS gates on evidence

Imagility is the closest **one-product** match to firm identity: named **O-1, H-1B, EB-1/2/3, I-140**, also **I-130/I-485**, petition scoring, RFE builder, beneficiary profiles, petitioner portal, mobile apps, some cap/bulk talk.

It is #7 as **CMS** because USCIS e-file is **2** (directory claim, no form list) and e-file was a kill criterion; case-status is events in the app, **not** USCIS receipt sync; Google is directory-only; admin configuration is **NS**; pricing is contact-sales. That is a poor fit for “live in weeks, no structured system today.”

**Use:** dark-horse demo **if** they can show org-account e-file and a family AOS bundle. Otherwise it is an expensive overlap with Parley/CaseBlink, not a system of record.

### 8. LollyLaw — good small-firm Google CMS, fails the e-file gate

Questionnaires (**4**), contact reuse into forms (**4**), 40 workflows, Gmail add-on, client portal. Family is thin in public docs. **USCIS e-file is NS**; filing is PDF + Chrome DS-160/260. Government e-file was required. Out as primary unless a demo shows USCIS online filing the report missed.

### 9. CampLegal — same story, clearer miss

Milestone CMS, conditional intakes, SMS, public SMB pricing. Filing is **auto-generated PDFs; no online filing evidence (2)**. Out as CMS.

### 10. INSZoom — right for a different buyer

Strongest **corporate / cap-season / LCA / HR** platform in the table. This buyer is a small firm, Google-first, weeks-not-months, **family AOS bundle is a must**, and O-1/EB-1 is the identity. Public family coverage is **NS**. Implementation is Mitratech-shaped, pricing is contact-sales. Cap registration is **not** the 90-day job (people and questionnaires stored is enough). Do not buy this to get off spreadsheets this quarter.

### 11. BlueDot — status toy, not the CMS

Direct USCIS API status (**4**) and relatively clear AI no-training language. E-file **2**, Outlook not Google, no petition drafting, no exhibit brain. Status was wanted **inside** the CMS already picked, not a second tracker with a weak forms engine.

### 12. Filevine ImmigrationAI — general PM tax not worth paying

Best public API and security package in the report. Immigration forms **2**, no e-file, **no named case types**, no family, no cap, no HR, implementation is a platform project. This is not a mid-large Filevine shop. Out.

### 13–17. Not CMS, ranked only as extras

| Rank | Product | Role |
| --- | --- | --- |
| Add-on A | **Parley** | Already in stacks 1 and 4. Best form-round-trip + RFE + voice fit. |
| Add-on B | **CaseBlink** | Stack 2. Best O-1/EB-1A specialist. |
| Pass as CMS / weak add-on | **Visalaw.ai** | Letters and research only. Use only if the form-round-trip requirement is dropped. |
| Pass | **Lawfully Pro** | Status was wanted **in the CMS**. Only a patch if Docketwise/eIMMIGRATION sync disappoints in demo. |
| Pass | **Inception AI / Formally** | Employment-AI claims, no e-file, no CMS, almost nothing verifiable. |
| Out | **OpenSphere** | DTC filing marketplace, not a firm system of record. |
| Out | **LawLogix Edge** | Stale public footprint, contact-sales, family/consular **NS**, not a weeks-long implementation. |

## If only three names

1. **Docketwise** — CMS the firm can actually run this quarter, including the family bundle and USCIS e-file.
2. **Parley** — the O-1/EB-1/NIW drafting + form-fill + RFE + exhibits layer.
3. **eIMMIGRATION** — backup CMS if Docketwise’s packets/Drive story loses the demo.

Legal Bridge and Imagility are **demo-only dark horses**, not paper winners.

## Demo script

Run the **same two matters** in every CMS trial:

1. **O-1A or EB-1A:** petitioner is a company, beneficiary uploads evidence, paralegal builds exhibits, attorney revises the letter, G-28 + I-129 or I-140, premium processing if used, export a packet, **e-file or show the exact org-account path**.
2. **Family AOS:** one person record fills **I-130 + I-485 + I-765 + I-131** without re-keying, questionnaire in the portal, mailed PDF packet with barcode fidelity.

Then, in the drafting tool:

3. Drop **one real prior winning petition** (redact if needed). Ask it to draft the next similar letter in that voice.
4. Drop a **real RFE**. Ask it to split requests and map them to the exhibit set.
5. Confirm whether filled USCIS forms **round-trip** into the CMS e-file path, or whether PDFs are carried by hand.

Kill tests:

- No USCIS e-file path for a form the firm actually files → CMS is out.
- AOS requires duplicate entry → CMS is out.
- AI only rewrites prose and will not fill I-129/I-140 → it fails the add-on bar.
- Gmail cannot file to the matter → serious ding (the firm lives in Google).
- Receipt sync is “we’ll scrape it” with no mechanism → status-in-CMS will not happen.

## What would still move the order

Not asked in the interview; would change weights:

- **Languages** other than English (Docketwise **5**, eIMMIGRATION **4**; most AI tools **NS**).
- **LCA/FLAG in the CMS** this year (Docketwise documents DOL e-file; it was not required).
- **E-sign in week one** (Docketwise native; left out of the 90-day list).
- A hard rule of **one vendor only** (then Legal Bridge/Imagility rise and Parley cannot win).
- Proof in demo that **Parley → Docketwise e-file** is painful (then eIMMIGRATION packets, or Legal Bridge-as-CMS, move up).

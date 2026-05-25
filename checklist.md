# GDPR Compliance Checklist — Automation Service Business

> **Your role in GDPR terms**
> - **Processor** (Art. 4(8), Art. 28) — when you process personal data on behalf of a client (their data, their customers' data, data pulled from their subscribed services).
> - **Sub-processor** — when you run automations on a client's premise infra you don't fully control, or when you use cloud/hosting providers under you.
> - **Controller** (Art. 4(7)) — only for data you decide the purposes of yourself: your own employees, prospects, billing contacts, website visitors.
> - **Joint controller** (Art. 26) — rare, only if you and a client jointly determine purposes/means. Avoid by contract unless intended.

Assume strict interpretation: every "should" below is treated as a "must".

---

## 1. Governance & accountability (Art. 5(2), 24)

- [ ] Written internal data protection policy approved by management.
- [ ] Named person accountable for GDPR internally (even if no formal DPO).
- [ ] **DPO appointed (Art. 37)** if core activities involve large-scale, regular & systematic monitoring or large-scale special-category data. For an automation provider handling many clients' customer data at scale → appoint one or document the reasoned decision not to.
- [ ] **EU representative (Art. 27)** if you are established outside the EU but offer services to EU data subjects.
- [ ] Annual compliance review documented.
- [ ] Staff GDPR training at onboarding + yearly refresher, attendance logged.
- [ ] Confidentiality / NDA clauses signed by every employee and contractor with data access (Art. 28(3)(b), Art. 29, Art. 32(4)).

---

## 2. Records of Processing Activities — RoPA (Art. 30)

Two separate registers:

### 2a. As **controller** (Art. 30(1)) — your own data
- [ ] Employees / HR records.
- [ ] Recruitment candidates.
- [ ] Customers (your client companies' billing/admin contacts).
- [ ] Prospects, CRM, marketing leads.
- [ ] Website visitors / cookies / analytics.
For each: purpose, legal basis, categories of data, categories of subjects, recipients, retention, transfers, security measures.

### 2b. As **processor** (Art. 30(2)) — per client
- [ ] One entry per client / per automation project.
- [ ] Name + contact of controller (client) and their DPO if any.
- [ ] Categories of processing performed (what the automation actually does).
- [ ] Sub-processors used (cloud, monitoring, error tracking, LLM APIs, etc.).
- [ ] International transfers + safeguards.
- [ ] Description of technical/organisational security measures (Art. 32).

- [ ] RoPA stored, versioned, available to supervisory authority on request.

---

## 3. Lawful basis & purpose (Art. 5, 6, 9, 10)

- [ ] For every automation, the **controller (client) has identified the lawful basis** — captured in writing in the contract/intake form.
- [ ] You do **not** repurpose client data for your own use (training models, analytics, marketing) without separate documented basis.
- [ ] **Special category data** (Art. 9 — health, biometrics, religion, political, union, sex life, genetic) flagged explicitly; processing refused or requires Art. 9(2) condition documented.
- [ ] **Criminal conviction data** (Art. 10) — refuse unless lawful authority.
- [ ] **Automated decision-making / profiling with legal or similarly significant effects (Art. 22)** — flagged; client must have safeguards (human review, right to contest, info notice). If your automation makes such decisions, contract makes this explicit.
- [ ] **Data minimisation** (Art. 5(1)(c)) — each automation pulls only the fields it needs; over-broad API scopes rejected.
- [ ] **Purpose limitation** (Art. 5(1)(b)) — written scope of processing per project; changes require change request.

---

## 4. Data Processing Agreement with every client (Art. 28)

A signed **DPA** before any production data touches your systems. Must contain Art. 28(3)(a)–(h):

- [ ] Subject-matter, duration, nature & purpose of processing.
- [ ] Types of personal data and categories of subjects.
- [ ] Obligations and rights of the controller.
- [ ] Processor acts **only on documented instructions** from controller (including transfers).
- [ ] Confidentiality of personnel.
- [ ] Security measures (Art. 32) — reference your technical & organisational measures (TOMs) annex.
- [ ] **Sub-processor terms**: general or specific written authorisation; notice of changes; flow-down obligations (Art. 28(2), 28(4)).
- [ ] Assistance with data subject rights (Art. 12–22).
- [ ] Assistance with security, breach notification, DPIA, prior consultation (Art. 32–36).
- [ ] Deletion or return of all personal data at end of contract; deletion of copies (with documented timeline).
- [ ] Audit & inspection rights for the controller.
- [ ] If automation runs on client premises: clarify who is responsible for which security layer; if you maintain remote access, that's still processing.
- [ ] DPA template reviewed by legal counsel.

---

## 5. Sub-processors (Art. 28(2), 28(4))

- [ ] Public, up-to-date list of all sub-processors (hosting, EU server provider, error monitoring, email, LLM/AI APIs, ticketing, backup, etc.).
- [ ] Each sub-processor under a contract with **equivalent** GDPR obligations.
- [ ] Due diligence file per sub-processor: GDPR posture, certifications (ISO 27001, SOC 2), location, transfer safeguards.
- [ ] Mechanism to notify clients of new/replaced sub-processors with right to object (e.g., 30 days).
- [ ] LLM / generative-AI vendors: contractually no training on input data; data residency confirmed.

---

## 6. International transfers (Ch. 5, Art. 44–49)

- [ ] Default: process and store in **EU/EEA**.
- [ ] Any transfer outside EU/EEA mapped: country, recipient, data categories, purpose.
- [ ] For each non-adequate country: **SCCs (2021/914)** signed + **Transfer Impact Assessment (TIA)** documented (post-Schrems II).
- [ ] Supplementary measures where needed (encryption with keys held in EU, pseudonymisation).
- [ ] US recipients: rely on **EU–US Data Privacy Framework** certification where applicable, otherwise SCCs + TIA.
- [ ] No transfers based on Art. 49 derogations except truly occasional cases, documented.

---

## 7. Security of processing (Art. 32) — TOMs

Document and apply, proportionate to risk:

- [ ] Encryption in transit (TLS 1.2+) for all data flows, including to client APIs.
- [ ] Encryption at rest for databases, backups, object storage.
- [ ] Secrets management (vault, never in code/repo); rotation policy.
- [ ] Strong authentication: MFA mandatory for all staff, all admin consoles, all client systems you access.
- [ ] Least-privilege RBAC; named accounts, no shared credentials.
- [ ] Network segregation between clients; one tenant cannot reach another.
- [ ] Hardened servers: patching SLA, CIS baseline, host firewall, EDR.
- [ ] Centralised, tamper-evident logging of access to personal data; retention sufficient for breach investigation.
- [ ] Backup + restore tested at least annually; backup encryption; documented RPO/RTO.
- [ ] Vulnerability scanning, dependency scanning, annual penetration test.
- [ ] Secure SDLC: code review, secret-scanning, SAST in CI.
- [ ] Endpoint security on developer laptops: disk encryption, MDM, screen lock.
- [ ] Physical security for any office where data is accessible.
- [ ] Incident response plan, tested at least yearly.
- [ ] When automation runs on **client premises**: written security baseline; remote access via jump host with MFA + session logging; clear demarcation of responsibilities; you do not store client data outside that environment unless authorised.

---

## 8. Privacy by Design and by Default (Art. 25)

- [ ] Privacy reviewed at project intake (template questionnaire).
- [ ] Default config minimises data collection and retention.
- [ ] Pseudonymisation / anonymisation used where the automation allows.
- [ ] Test/staging environments do **not** use real personal data, or use masked/synthetic data.
- [ ] Logs do not contain unnecessary personal data; PII redaction in error monitoring.

---

## 9. Data Protection Impact Assessment — DPIA (Art. 35)

- [ ] DPIA triggered checklist applied to every new automation: large-scale processing, systematic monitoring, special categories, automated decisions with significant effect, new technologies (incl. AI/LLMs), combining datasets, vulnerable subjects.
- [ ] DPIA template (description, necessity, proportionality, risks, mitigations).
- [ ] DPO consulted (if any); supervisory authority consulted (Art. 36) if residual high risk.
- [ ] DPIA stored with the project's RoPA entry.

---

## 10. Data subject rights — support as processor (Art. 12–22, 28(3)(e))

You typically forward requests to the controller, but must be able to act fast:

- [ ] Documented procedure: when a data subject contacts you directly → redirect to controller; when the controller forwards a request → respond within agreed SLA (< 30 days minus client handling time).
- [ ] Tooling to fulfil each right per client dataset:
  - [ ] Access (Art. 15) — export of all data on a subject.
  - [ ] Rectification (Art. 16).
  - [ ] Erasure / right to be forgotten (Art. 17) — including from backups (documented approach).
  - [ ] Restriction (Art. 18).
  - [ ] Portability (Art. 20) — machine-readable export.
  - [ ] Objection (Art. 21).
  - [ ] Not to be subject to solely automated decisions (Art. 22).
- [ ] Identity-verification process before acting on a request.

---

## 11. Breach management (Art. 33, 34)

- [ ] Internal incident classification with a "personal data breach" branch.
- [ ] **As processor: notify controller without undue delay** after becoming aware (Art. 33(2)). Target: hours, not days. Defined in DPA.
- [ ] As controller (own data): notify your supervisory authority within **72 hours** (Art. 33(1)).
- [ ] Notify affected data subjects when high risk (Art. 34).
- [ ] Breach register: all incidents, including those not notified, with reasoning.
- [ ] Post-incident review and corrective actions tracked.

---

## 12. Transparency (Art. 12–14) — for data you control directly

- [ ] Public privacy notice on your website covering: identity, DPO contact, purposes, legal basis, recipients, transfers, retention, data subject rights, right to complain to a supervisory authority, source of data (if not from subject).
- [ ] Separate notice / information layer for employees, candidates.
- [ ] Cookie banner compliant with ePrivacy + GDPR consent (Art. 7) — granular, refusable, no pre-ticked boxes, easy withdrawal.
- [ ] Marketing emails: lawful basis (consent or soft opt-in where allowed), unsubscribe link, sender identification.

---

## 13. Retention & deletion (Art. 5(1)(e), 17)

- [ ] Retention schedule per category of data, per client.
- [ ] Automated deletion / archival jobs; evidence of execution.
- [ ] End-of-contract: documented process to return or delete client data within X days, certificate of deletion issued.
- [ ] Backup retention policy aligned (e.g., rolling 30/90 days, then purged).

---

## 14. Contracts & sales process

- [ ] No client onboarding without: signed MSA + signed DPA + (if applicable) SCCs + sub-processor disclosure.
- [ ] Pre-sales questionnaire flags special categories, Art. 22 automation, large-scale monitoring → triggers DPIA before go-live.
- [ ] Change-request process if scope of processing changes mid-contract.
- [ ] Client given a TOM (Technical & Organisational Measures) document and sub-processor list as annexes.

---

## 15. Cooperation with authorities (Art. 31, 58)

- [ ] Identify your **lead supervisory authority** (country of main establishment in the EU).
- [ ] Process to respond to authority requests; legal counsel on retainer.
- [ ] Records of any prior consultations or investigations.

---

## 16. Specific to your business model — high-risk areas to lock down

- [ ] **Access to client's third-party services** (e.g., their SaaS subscriptions): use the client's own credentials/OAuth grants, never share across clients, store tokens encrypted, principle of least scope, revoke at offboarding.
- [ ] **Data pulled from client's clients (end-users)**: confirm in DPA that the client has the lawful basis and has informed those end-users that a processor (you) is involved.
- [ ] **Automations on EU server (your premise)**: it is *your* infrastructure → you are responsible for all of Art. 32; document tenancy isolation.
- [ ] **Automations on client premise**: clarify in DPA — you are still a processor for what you remotely operate; client controls the physical/network layer; security responsibility matrix attached.
- [ ] **AI / LLM components**: if you send personal data to an LLM API, that vendor is a sub-processor; ensure no-training clause, EU region, DPA in place; consider DPIA; prefer pseudonymisation before sending.
- [ ] **Logs & observability**: PII scrubbing; access restricted; same retention rules as production data.
- [ ] **Developer access to production data**: forbidden by default; break-glass procedure with approval + logging.
- [ ] **Offboarding checklist per client**: revoke all access, delete or return all data, rotate any shared secrets, archive RoPA entry, issue deletion certificate.

---

## 17. Evidence pack (what you must be able to produce on day one of an audit)

- [ ] RoPA (controller + processor).
- [ ] DPA template + signed DPAs per client.
- [ ] Sub-processor list + agreements.
- [ ] TOMs document.
- [ ] Information security policy, incident response plan, breach register.
- [ ] DPIA register + completed DPIAs.
- [ ] Training records.
- [ ] Transfer mapping + SCCs + TIAs.
- [ ] Data subject request log.
- [ ] Retention schedule + deletion evidence.
- [ ] Privacy notices (current and historical versions).

---

### Fine exposure reminder (Art. 83)
- Up to **€10M or 2%** of global annual turnover (e.g. RoPA, security, breach notification failings).
- Up to **€20M or 4%** of global annual turnover (e.g. lawful basis, data subject rights, international transfers).
Whichever is higher.

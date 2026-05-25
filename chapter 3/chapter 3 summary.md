# Chapter 3 GDPR – Rights of the Data Subject (Art. 12–23)

## Overview

Chapter 3 is the **data subject rights chapter** — the practical heart of GDPR from an individual's perspective. It grants natural persons a comprehensive set of enforceable rights against controllers, and imposes corresponding obligations on controllers to respond transparently, promptly, and free of charge. The chapter is organised into five sections:

| Section | Topic | Articles |
|---------|-------|---------|
| 1 | Transparency & modalities | Art. 12 |
| 2 | Information & access | Art. 13–15 |
| 3 | Rectification & erasure | Art. 16–20 |
| 4 | Right to object & automated decisions | Art. 21–22 |
| 5 | Restrictions | Art. 23 |

---

## Article Summaries

### Art. 12 – Transparent Information, Communication and Modalities
The procedural backbone of the chapter. Controllers must communicate with data subjects in **clear, plain, and concise language**. Responses to rights requests (Art. 15–22) must be provided **within one month** (extendable by two more months for complex cases). Responses are **free of charge** unless requests are manifestly unfounded or excessive. Controllers may request additional information to verify identity before acting.

### Art. 13 – Information to Be Provided Where Data Are Collected from the Data Subject
When data are collected directly from the data subject, the controller must provide a **privacy notice at the time of collection** covering: identity of the controller (and DPO), purposes and legal basis, legitimate interests (if applicable), recipients, third-country transfer safeguards, retention periods, all applicable data subject rights, right to withdraw consent, right to lodge a complaint, and whether provision is mandatory. Additional notice is required before any further-purpose processing.

### Art. 14 – Information to Be Provided Where Data Have Not Been Obtained from the Data Subject
Mirrors Art. 13 but applies where data come from **third-party sources**. The controller must additionally disclose the **source** of the data. Notice must be given within **one month** of obtaining the data (or at first contact / first disclosure, whichever is earlier). Exceptions exist for impossibility, disproportionate effort, legal secrecy obligations, and existing knowledge.

### Art. 15 – Right of Access
Data subjects may request **confirmation** of whether their data is being processed and, if so, receive a **copy** of the data plus supplementary information (purposes, categories, recipients, retention, rights, third-country safeguards, automated-decision logic). The first copy is free; subsequent copies may attract a fee. The right must not adversely affect others' rights and freedoms.

### Art. 16 – Right to Rectification
Data subjects can demand **correction of inaccurate data** and **completion of incomplete data** without undue delay. Controllers must act promptly and propagate corrections to any recipients under Art. 19.

### Art. 17 – Right to Erasure ('Right to Be Forgotten')
Data subjects may request deletion where data are **no longer necessary**, **consent is withdrawn** (and no other basis exists), **processing was unlawful**, or **an objection succeeds**. Where data have been made public, the controller must take reasonable steps to inform other controllers. Six exceptions preserve data for freedom of expression, legal obligations, public health, archiving/research, and legal claims.

### Art. 18 – Right to Restriction of Processing
Instead of erasure, a data subject may request that processing be **frozen** (data retained but not used) in four situations: contested accuracy, unlawful processing where erasure is opposed, data needed for legal claims, or pending verification of an Art. 21 objection. The controller must inform the data subject before lifting a restriction.

### Art. 19 – Notification Obligation
When a controller carries out rectification, erasure, or restriction under Art. 16–18, it must **notify all recipients** to whom the data were disclosed — unless this is impossible or disproportionate. The controller must inform the data subject of those recipients upon request.

### Art. 20 – Right to Data Portability
Data subjects have the right to receive their data in a **structured, commonly used, machine-readable format** and to transmit it directly to another controller. Applies only where processing is based on **consent or contract** and is carried out **by automated means**. Does not apply to public-interest/official-authority processing and must not prejudice others' rights.

### Art. 21 – Right to Object
Data subjects may object at any time to processing based on **public task (Art. 6(1)(e)) or legitimate interests (Art. 6(1)(f))**, including profiling. The controller must cease processing unless it can demonstrate compelling legitimate grounds. For **direct marketing**, the right is absolute — no override is possible. The right must be **explicitly communicated** to data subjects at first contact, separately from other information.

### Art. 22 – Automated Individual Decision-Making, Including Profiling
Data subjects have the right not to be subject to **solely automated decisions** that produce legal or similarly significant effects. Exceptions: contract necessity, legal authorisation, or **explicit consent**. Where an exception applies, the controller must implement human intervention, the right to express a point of view, and the right to contest. Automated decisions based on **special-category data** are prohibited unless Art. 9(2)(a) or (g) applies.

### Art. 23 – Restrictions
Union or Member State law may **restrict data subject rights (Art. 12–22) and Art. 5 obligations** where necessary and proportionate to safeguard national security, defence, public security, crime prevention/prosecution, important public interests, judicial independence, professional ethics oversight, monitoring/regulatory functions, data subject protection, or civil law enforcement. Any such restriction must contain specific safeguard provisions (purposes, categories, scope, safeguards, controllers, retention, risks, notification right).

---

## Chapter-level Todo List

- [ ] Establish a **data subject rights intake process** (logging, acknowledgement, deadline tracking) covering all rights in Art. 15–22.
- [ ] Ensure all responses to rights requests comply with Art. 12 timeframes (1 month, extendable by 2 months) and are free of charge.
- [ ] Build or update **privacy notices** for direct data collection (Art. 13) covering all mandatory elements.
- [ ] Build or update **privacy notices** for indirectly obtained data (Art. 14) including source disclosure and delivery deadlines.
- [ ] Implement a process to respond to **access requests** (Art. 15) and provide data copies in a usable format.
- [ ] Implement a **rectification workflow** that propagates corrections to downstream recipients (Art. 16 + 19).
- [ ] Implement an **erasure workflow** ('right to be forgotten', Art. 17) including notifying third-party controllers where data was made public.
- [ ] Implement a **restriction-of-processing** flag/mechanism in systems (Art. 18).
- [ ] Build a **data portability export** feature for consent/contract-based automated processing (Art. 20).
- [ ] Display a clear, prominent **right-to-object notice** in all relevant communications, especially for direct marketing (Art. 21).
- [ ] Map all **automated decision-making** processes; implement human review, contest mechanisms, and meaningful logic explanations (Art. 22).
- [ ] Review applicable Union/Member State law for any permissible **restrictions** (Art. 23) and document them.
- [ ] Train staff on responding to data subject requests, including identity verification and when to refuse or charge a fee (Art. 12).
- [ ] Conduct DPIAs for high-risk automated decision-making and profiling activities (Art. 22).

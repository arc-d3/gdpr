# Art. 21 GDPR – Right to Object

## Summary

Article 21 gives data subjects the right to **object at any time** to certain processing activities, with varying strength depending on the purpose.

### Paragraph 1 — General Right to Object (Art. 6(1)(e)/(f) legal bases)
A data subject may object to processing based on **public task (Art. 6(1)(e))** or **legitimate interests (Art. 6(1)(f))**, including profiling on those bases.

- The controller must **stop processing** unless it can demonstrate **compelling legitimate grounds** that override the data subject's interests, rights, and freedoms, or the processing is for the establishment, exercise, or defence of **legal claims**.
- The burden of proof lies with the **controller**.

### Paragraph 2 — Absolute Right: Direct Marketing
Where data are processed for **direct marketing** purposes (including related profiling):
- The data subject may object **at any time**.
- The right is **absolute** — no override by the controller is possible.
- Upon objection, processing for direct marketing **must cease immediately**.

### Paragraph 3 — Effect of Objection to Direct Marketing
Once a data subject objects to direct marketing processing, data may **no longer be used** for that purpose.

### Paragraph 4 — Notice Obligation
The right to object must be **explicitly brought to the attention** of the data subject **at the latest at the time of the first communication**, clearly and **separately from any other information**.

### Paragraph 5 — Automated Objection
In the context of information society services, data subjects may exercise the right to object by **automated means using technical specifications** (e.g., browser settings, opt-out signals).

### Paragraph 6 — Research/Statistical Purposes
Data subjects may object to processing for **scientific/historical research or statistical purposes** (Art. 89(1)) based on their particular situation, unless the processing is necessary for a **public-interest task**.

---

## Todo List

- [ ] Identify all processing activities based on **Art. 6(1)(e) or (f)** (public task / legitimate interests) and ensure objection handling procedures exist for each.
- [ ] Implement an **objection intake workflow** that, upon receipt, immediately restricts processing pending assessment of compelling legitimate grounds.
- [ ] Document the legal assessment process for determining whether **compelling legitimate grounds** override the data subject's objection; obtain legal sign-off.
- [ ] For all **direct marketing processing**, implement an **unconditional opt-out mechanism** that ceases processing immediately and propagates to all channels.
- [ ] Audit all outbound marketing communications to ensure the **right to object is prominently and separately disclosed** at first contact (Art. 21(4)).
- [ ] Implement **automated opt-out / unsubscribe mechanisms** compatible with technical specifications (e.g., List-Unsubscribe headers, Global Privacy Control).
- [ ] Review and update CRM and marketing systems to ensure objection flags are **honoured across all touchpoints** (email, SMS, phone, ads).
- [ ] Clearly communicate the right to object in privacy notices (Art. 13/14 requirement).
- [ ] Log all objections received, grounds assessed, and outcomes for accountability purposes.
- [ ] Apply Art. 12 response deadlines (one month, extendable) to objection requests that require a formal grounds-assessment response.

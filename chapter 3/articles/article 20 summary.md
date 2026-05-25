# Art. 20 GDPR – Right to Data Portability

## Summary

Article 20 gives data subjects the right to **receive their personal data in a portable format** and to **transmit it to another controller** — facilitating freedom of choice and competition between service providers.

### Paragraph 1 — Scope
The right applies where **all three conditions** are met:

| Condition | Requirement |
|-----------|-------------|
| **Legal basis** | Processing is based on **consent** (Art. 6(1)(a) or Art. 9(2)(a)) or on a **contract** (Art. 6(1)(b)). |
| **Automated means** | The processing is carried out **by automated means** (not manual paper-based processing). |
| **Data provided by the subject** | The data were **provided by the data subject** to the controller. |

The data must be provided in a **structured, commonly used, and machine-readable format** (e.g., JSON, CSV, XML).

### Paragraph 2 — Direct Transmission
Where technically feasible, the data subject may request that data be transmitted **directly from one controller to another**.

### Paragraphs 3–4 — Limits
- The portability right is **without prejudice to Art. 17** (erasure right — exercising portability does not prevent the data subject from also requesting erasure).
- The right does **not apply** to processing necessary for the performance of a **public task or official authority**.
- Exercise of the right must **not adversely affect** the rights and freedoms of others.

---

## Todo List

- [ ] Identify all processing activities based on **consent or contract** that use **automated means** — these are in scope for Art. 20.
- [ ] Build a **data export feature** that produces a structured, commonly used, machine-readable format (e.g., JSON or CSV) for all in-scope data.
- [ ] Assess technical feasibility of **direct controller-to-controller data transmission** (e.g., via API); implement or document the plan.
- [ ] Ensure the export does not include data that would **adversely affect others' rights** (e.g., third-party personal data intermingled with the data subject's data).
- [ ] Integrate portability into the general **rights request intake workflow** (Art. 12 deadlines apply).
- [ ] Clearly communicate the right to data portability in privacy notices (required by Art. 13/14).
- [ ] Document which processing activities are **excluded** from portability (public task / official authority) and train staff accordingly.
- [ ] Log all portability requests, data provided, and any refusals with reasons for accountability purposes.
- [ ] Review and test the export format against common open standards to ensure interoperability with receiving controllers.

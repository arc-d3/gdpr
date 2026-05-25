# Art. 17 GDPR – Right to Erasure ('Right to Be Forgotten')

## Summary

Article 17 gives data subjects the right to obtain **deletion of their personal data without undue delay** when one of six grounds applies.

### Paragraph 1 — Grounds for Erasure

| Ground | Description |
|--------|-------------|
| (a) | Data are **no longer necessary** for the purpose for which they were collected or processed. |
| (b) | Data subject **withdraws consent** (Art. 6(1)(a) or Art. 9(2)(a)) and no other legal basis exists. |
| (c) | Data subject **objects** under Art. 21(1) and no overriding legitimate grounds exist, or objects under Art. 21(2) (direct marketing). |
| (d) | Personal data have been **unlawfully processed**. |
| (e) | Erasure required to comply with a **legal obligation** under Union or Member State law. |
| (f) | Data collected in relation to the offer of **information society services to a child** (Art. 8(1)). |

### Paragraph 2 — Public Data ('Right to Be Forgotten')
Where the controller has **made the data public** and is obliged to erase it, the controller must take **reasonable steps** (taking into account available technology and implementation cost) to inform other controllers processing the data that the data subject has requested erasure — including erasure of links, copies, and replications.

### Paragraph 3 — Exceptions (erasure does **not** apply if processing is necessary for)

| Exception |
|-----------|
| (a) Exercising the right of **freedom of expression and information** |
| (b) Compliance with a **legal obligation** or performance of a task in the **public interest / official authority** |
| (c) **Public health** purposes (Art. 9(2)(h)(i) and Art. 9(3)) |
| (d) **Archiving, scientific/historical research, or statistical purposes** (Art. 89(1)) where erasure would seriously impair objectives |
| (e) Establishment, exercise, or defence of **legal claims** |

---

## Todo List

- [ ] Implement an **erasure request workflow** (online + offline) that evaluates all six grounds in Art. 17(1).
- [ ] Build a **grounds-assessment checklist** so that responding staff can systematically evaluate whether an erasure exception under Art. 17(3) applies.
- [ ] Ensure technical capability to **delete data from all systems** — databases, backups, archives, logs, third-party processors — on receipt of a valid erasure request.
- [ ] Implement the **"right to be forgotten" cascade**: where data were made public, build a process to notify other controllers (e.g., search engines, partner sites) of the erasure obligation.
- [ ] Link the erasure workflow to the **Art. 19 notification process** to inform recipients/processors who received the data.
- [ ] Define and document **retention policies** that distinguish between business retention (limiting grounds for erasure) and legally mandated retention (exception under Art. 17(3)(b)).
- [ ] Apply Art. 12 response deadlines (one month, extendable) to all erasure requests.
- [ ] Log all erasure requests, decisions, exceptions relied upon, and actions taken for accountability purposes.
- [ ] Review privacy notices to ensure the right to erasure is clearly communicated (required by Art. 13/14).
- [ ] Ensure consent-withdrawal mechanisms automatically trigger an erasure assessment where consent is the sole legal basis.

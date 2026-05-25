# Art. 18 GDPR – Right to Restriction of Processing

## Summary

Article 18 grants data subjects the right to obtain a **freeze on the use** of their personal data (while the data is retained) in four specific circumstances. During restriction, data may only be stored; further processing requires consent, legal claims, protection of others, or important public interest.

### Paragraph 1 — Grounds for Restriction

| Ground | When it applies |
|--------|----------------|
| (a) **Accuracy contested** | The data subject disputes the accuracy of the data — restriction applies for the period needed to verify accuracy. |
| (b) **Unlawful processing, erasure opposed** | Processing is unlawful but the data subject prefers restriction over erasure (e.g., to preserve it for legal claims). |
| (c) **Data needed for legal claims** | The controller no longer needs the data, but the data subject requires it for establishing, exercising, or defending legal claims. |
| (d) **Pending Art. 21 objection** | The data subject has objected under Art. 21(1) and verification of overriding grounds is pending. |

### Paragraph 2 — Effect of Restriction
During restriction, data may only be processed (beyond mere storage) for:
- The data subject's **consent**;
- Establishment, exercise, or defence of **legal claims**;
- Protection of the **rights of another natural or legal person**; or
- **Important public interest** of the Union or a Member State.

### Paragraph 3 — Lifting the Restriction
Before lifting a restriction, the controller must **inform the data subject** in advance.

---

## Todo List

- [ ] Implement a **restriction request workflow** accessible to data subjects; distinguish from erasure requests in the intake form.
- [ ] Build a technical **"restricted" flag or status** in key data systems so that restricted records are excluded from processing operations (queries, exports, analytics) while remaining stored.
- [ ] Ensure restricted data can still be accessed for the four permitted processing purposes (consent, legal claims, third-party protection, public interest).
- [ ] Create a process to **lift restrictions** when the grounds expire, with mandatory advance notification to the data subject.
- [ ] Link the restriction workflow to the **Art. 19 notification process** to inform recipients that processing of the data is restricted.
- [ ] Apply Art. 12 response deadlines (one month, extendable) to restriction requests.
- [ ] Log all restriction requests, grounds assessed, restriction start/end dates, and lifting notifications for accountability purposes.
- [ ] Review privacy notices to ensure the right to restriction is clearly communicated (required by Art. 13/14).
- [ ] Train staff on the difference between erasure and restriction, and when each applies.

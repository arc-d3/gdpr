# Art. 19 GDPR – Notification Obligation Regarding Rectification or Erasure of Personal Data or Restriction of Processing

## Summary

Article 19 is the **downstream notification duty** that flows from Art. 16 (rectification), Art. 17(1) (erasure), and Art. 18 (restriction). When a controller carries out any of these operations, it must propagate that change to all **recipients** who received the data.

| Obligation | Detail |
|------------|--------|
| **Notify recipients** | The controller must communicate rectification, erasure, or restriction to **each recipient** to whom the data were disclosed. |
| **Exception** | Notification is not required if it proves **impossible** or involves **disproportionate effort**. |
| **Inform the data subject** | The controller must inform the data subject of those recipients **if the data subject requests it**. |

The article is brief but critically important: without this cascade obligation, corrections or deletions at the source controller would leave inaccurate or unlawfully retained copies with third parties.

---

## Todo List

- [ ] Maintain a **recipient register** per data set / processing activity so that all downstream recipients can be identified quickly when rectification, erasure, or restriction occurs.
- [ ] Integrate the Art. 19 notification step into the **rectification, erasure, and restriction request workflows** (Art. 16, 17, 18) — it should trigger automatically upon completion.
- [ ] Define the **notification format and channel** for informing recipients (e.g., automated API call, secure email, data feed update).
- [ ] Establish and document the criteria for invoking the **impossibility / disproportionate effort** exception, with legal review approval.
- [ ] Log all recipient notifications sent under Art. 19 (recipient, date, nature of change) for accountability purposes.
- [ ] Ensure privacy notices inform data subjects of their right to receive information about recipients upon request (Art. 13/14 + Art. 19 link).
- [ ] Review contracts with processors and joint controllers to confirm Art. 19 notification obligations are flowed down contractually.
- [ ] Periodically audit the recipient register to keep it accurate and up to date.

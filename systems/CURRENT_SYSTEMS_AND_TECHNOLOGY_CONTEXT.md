# Current systems and technology context

**Mettelo Business Analyst Project Studio · MTL-BA-041 · Stage 3**  
**Source:** Oliver King's discovery note, 20 July 2026, with supplier correspondence  
Capabilities described as “possible”, “indicative” or “demonstrated” are not contracted or approved.

## 1. Current products and ownership

| Product/source | Current business use | Business owner | Technical/source limitation |
|---|---|---|---|
| OrderHub | Online order, basket, delivery reference and account lookup | Ecommerce | Nightly read-only export at 02:00 UK; no contracted return-status write-back |
| TillPoint | Store sales, branch refund authority and receipt | Store Operations | Branch close-of-day batches; online refunds cannot be released directly at till |
| ServiceDesk | Central return record, adviser contacts and customer macros | Customer Service | Adviser-selected status and configurable fields; receipt evidence is not always attached |
| DepotSheet | Parcel match, inspection note and stock disposition | Warehouse | Shared workbook; not every amendment has an attributable event history |
| FinancePay | Approved central instruction file, provider response and reconciliation | Finance | Separate batch/attempt references; responses need business review |
| Board workbook | Combined performance reporting | Finance | Cohort/completion definitions are easy to mislabel; not an operational work queue |

This is an inventory of current sources. It is not the participant's future architecture, conceptual data model or integration specification.

## 2. Identifiers and current record movement

OrderHub order IDs identify an order, not necessarily one returned item or one return case. ServiceDesk creates a central return ID. A store may first record custody against an order/item on paper and obtain the central ID later. DepotSheet can therefore contain a central return ID, an order number or a temporary parcel note.

The CSV evidence was assembled by the coordinator using existing links and documented manual matching. It is a reconciled analysis extract, not proof that the live platforms already share a clean universal key. A receipt_link_method of manual_match reports how the source records were linked; it is not an automatic error flag or an instruction to discard the row.

FinancePay uses a unique attempt reference and can submit a replacement after rejection. A replacement is not a new return. The source payment extract includes a blocked duplicate attempt for R0857. Neither an “accepted” response nor an adviser status proves the customer saw the money at the same time.

## 3. Interface and scheduling facts at discovery

OrderHub's nightly export is read-only under the current contract. The supplier has not committed to return-status write-back before the November freeze. Ecommerce's earlier demonstration used seeded immediate responses. Oliver has requested a written response about delivery options; the formal response appears only in the later change stage.

TillPoint exports arrive after each branch closes. A branch can be offline while its local paper record still exists. The warehouse workbook is exported at the end of the shift. FinancePay responses are imported into a reconciliation workspace independently of ServiceDesk. An alert to a technical mailbox does not confirm that all business exceptions have been resolved.

Some files are retried manually after a schema or reference error. No complete replay test has been supplied. There is no agreed tolerance for stale customer-visible status, no full missed-file reconciliation evidence and no proven end-to-end outage procedure in the materials received.

## 4. Current-tool capability claims

Oliver believes ServiceDesk can support an additional queue, controlled fields and a reference lookup. A supplier helpdesk confirmed those features exist in the licensed product, but did not validate Northbank's intended use. Configuration effort, access model, audit coverage, performance and support remain to be assessed.

A read-only combined view may be possible with current exports. It would still need agreed field meaning, record matching, ownership, update timing and exception handling. Physical inspection and a consumer-rights decision are not capabilities a screen can substitute for. The BA must establish the need and the acceptance evidence without prescribing unsupported technical details.

Internal capacity estimate: two analyst days per week for six weeks, plus four integration-specialist days, at planning rates of £450 and £650 per day respectively. These are indicative opportunity/backfill rates, not an approved booking or a complete option cost. September security patching competes for the same specialists.

## 5. Commercial material — unscored raw inputs

### Supplier FlowReturn — 16 July email

Hosted return portal and task queue. Setup £32,000; incremental subscription £12,000 per year for 30 named users; minimum 24-month term. Quote excludes OrderHub connector, data cleansing, branch devices, historical migration, training/backfill, VAT and independent assurance. Indicative connector allowance £18,000, subject to a signed interface specification. Supplier claims “up to 30% fewer refund-status calls” using an unspecified customer example; no comparable dataset was provided.

The supplier demonstrated customer lookup, adviser search and a queue. It did not demonstrate Northbank's store receipt, provider rejection, duplicate instruction, role restrictions or missed-file recovery. Supplier says these are configuration topics; Finance asks whether they are included in the price.

### Current-tools configuration — internal planning note, 17 July

Potentially retain ServiceDesk and build a controlled reference/exception view from existing exports. The effort inputs above are available for costing, but Operations has not released staff for discovery, data repair, training or validation. Additional annual support is estimated at £4,000–£7,000. No latency, audit, resilience or usability commitment has been approved.

### Broader replacement — unsolicited MarketSuite proposal, 18 July

Initial implementation from £58,000; annual licence from £22,000; minimum three-year term. Supplier claims cross-channel case management and analytics. No fixed integration scope, migration plan or branch demonstration is attached. The recurring quote exceeds the initial operating ceiling, but the BA must still explain relevant trade-offs rather than select an option from price alone.

These sources do not form a completed options appraisal. Do not adopt a supplier's benefit percentage or timeline as Northbank's business case. A process/policy-only intervention, sequenced approach or deferral can also be considered if justified by the participant.

## 6. Support, security and deployment considerations raised by IT

Oliver wants ownership of access, configuration, failed imports and the business consequences of a delayed file. A new application would need appropriate supplier/data review and an operational support route. Existing tools also require control review; remaining on an old product is not proof of safety.

A configuration change should be distinguishable from a policy change. Staff training, customer wording, historic open cases and rollback need attention whichever product is chosen. No production access, credentials or actual personal data are supplied. The August demonstration is isolated and uses synthetic records.

## 7. Matters not established

No source establishes final user count, connector scope, complete interface mapping, uptime or recovery targets, acceptable staleness, retention schedule, complete licence entitlements, realistic peak workload, total implementation cost or an approved support model. Those gaps affect decisions and should appear in the participant's analysis.

The BA is expected to turn business needs and constraints into testable requirements with appropriate technical collaboration. This document intentionally does not supply those requirements, service-level values, migration mappings or an architecture recommendation.

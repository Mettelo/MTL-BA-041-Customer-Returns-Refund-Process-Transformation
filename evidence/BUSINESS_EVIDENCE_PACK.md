# Business evidence pack — operational fragments and supporting records

**Mettelo Business Analyst Project Studio · MTL-BA-041 · Stage 3**  
**Collated:** 20 July 2026 · **Snapshot context:** April–June records  
All documents, observations and statements below are synthetic. Their purpose is to support investigation, not to supply a root-cause report.

## 1. Evidence register and limitations

BE01 is a short Service desk observation; BE02 a branch/depot observation; BE03 Finance exception notes; BE04 a limited assurance sample; BE05 customer/colleague correspondence; BE06 planning-cost inputs; BE07 data/records access notes. Each has a different author, scope and strength. A statement may be an observation, a recollection or an untested explanation.

The three linked CSVs are the operational source population defined in DATA_GUIDE.md. This pack adds context that cannot be inferred from dates alone. No complete process map, activity-cost model, gap analysis or options decision is supplied.

## 2. BE01 — Customer Service observation, 22 June, 09:00–10:30

**Observer:** programme coordinator, seated with one experienced adviser. This was not a representative time study.

09:08: a customer asks whether the store has received their return. The adviser finds the online order, then searches a separate mailbox for a branch photograph. The customer has a branch receipt; the central record has no attached copy. The adviser puts the customer on hold to contact a team leader.

09:23: another adviser asks whether “submitted” can be described as “paid”. The team leader says to use the approved macro but cannot identify the date of its last review. The macro refers to five working days after warehouse confirmation; the web page uses five days of receipt.

09:41: an adviser sees a Finance note with a batch reference and selects the refunded label. The observer cannot see a provider response in ServiceDesk. The adviser says Finance would tell them if it failed. No evidence of a rejection-notification control is produced during the session.

10:02: a store calls about a refund between £100 and £150. The adviser searches the Finance email while the store customer waits. The question is escalated to Service leadership. The observer does not verify the customer's entitlement or final decision.

The observed session includes call waiting, navigation and discussion but no reliable per-activity stopwatch record. It cannot establish a universal handling-time saving. The adviser says a second monitor would help; IT asks whether that addresses the missing facts or only screen switching.

## 3. BE02 — Branch and depot source fragments

### S07 branch desk note, 24 June

Jo's team keeps a paper acknowledgement pad beside the online lookup terminal. On a busy Saturday a colleague may write an order number, item description and initials before a central return ID exists. The original is given to the customer, with a duplicate retained locally. Some photographs of those duplicates are emailed to Service.

The transfer cage sheet groups parcels for the depot. It records a cage dispatch, not a precise scan for each return. The branch does not record a reliable case-level departure timestamp in the supplied extract. The coordinator cannot reconstruct the full physical custody history from the CSV alone.

### Depot bench note, 25 June

A colleague unpacks goods, checks an available reference, records an inspection note and moves the product to a resale, quarantine or disposal location. Identification queries can interrupt this work. A colleague may phone a branch or search the order list. Those interruptions are not consistently marked as rework.

Tom notes that inspection_recorded_date can be the date the workbook was updated after a shift, not the exact time the product was inspected. The extract's first_goods_received_date may refer to a branch days earlier. No evidence supports assigning the entire intervening interval to one team's active handling time.

### Selected source records

| Return | Receipt/source fact | Further event in frozen records | Unresolved source detail |
|---|---|---|---|
| R0851 | S07 accepted online homeware on 2 June | Inspection entry 9 June; Finance authorisation 11 June; accepted instruction 12 June | Item-level transfer history and complete branch evidence |
| R0855 | S07 accepted sealed personal-care goods on 3 June | Inspection 11 June; authorisation 15 June; accepted instruction 16 June | Whether disputed delegation was decisive, and who approved it |
| R0860 | S07 accepted wrong-item return on 5 June | Manual match; inspection 12 June; accepted instruction 17 June | How the colleague established the match and what was communicated |

This table is a source index for selected cases, not a cause finding or a completed exception process.

## 4. BE03 — Finance exception desk note, 30 June

Priya supplied the following observations with references to the payment extract:

- R0852 / PAY00875: £119 instruction rejected on 19 June as payment_token_invalid. PAY00876 replaces it on 23 June, is accepted and has a 26 June settlement confirmation. The source does not show when Service or the customer first learned of the rejection.
- R0857 / PAY00880: £399 accepted on 11 June. PAY00881 was blocked the same day as duplicate_reference. The Finance note says “check double submission”; it does not report two settled payments or a £399 duplicate loss.
- R0851 / PAY00874: £149 accepted on 12 June. There is no settlement confirmation retained in this frozen extract. That is an evidence gap; it does not by itself prove the customer remained unpaid at cutoff.
- R0856: £79 request is still marked policy_query after inspection. No Finance authorisation or payment attempt is observed. The opened-seal category requires facts and policy review; no legal eligibility conclusion was supplied.

Finance batches can contain several returns. An export that runs without a technical error can still contain business rejections. Priya asks whether a future approach would preserve the original attempt, relationship to a retry, reason, reviewer and eventual communication. This is a question for analysis, not an approved requirement record.

## 5. BE04 — limited internal assurance review

**Author:** internal assurance associate · **Review date:** 26 June  
**Selection:** 36 central refund files first authorised between 1 and 19 June, chosen from a local worklist for document availability. The exact 36-file list was not retained in the material supplied to the BA. It cannot be joined reliably to the full CSV or used as a statistically representative error rate.

Findings in the associate's notes: 7 of 36 files lacked an attributable inspection/evidence attachment in the reviewed folder; 5 lacked a retained policy-version reference; 4 had an adviser “refunded” label before the first accepted provider instruction. Categories overlap, so counts must not be added as distinct affected cases.

The review did not determine whether missing attachments existed elsewhere, whether every authorisation was valid, whether a customer-rights deadline was missed, or whether any money was paid twice. Assurance requested source retrieval and clarified document ownership before a broader review. No control certification or legal finding was issued.

**Management responses:** Tom says inspection information may remain in DepotSheet rather than the Finance folder. Aisha says the label problem is training and screen wording. Priya says dispersed evidence still makes audit and reconciliation harder. Helen asks whether a new platform would make evidence capture mandatory; Jo asks how that would work at an offline counter.

These responses do not establish a single agreed cause.

## 6. BE05 — communications and case accounts

### Customer account linked to R0851

“The store took the item on 2 June. I still had a slip when your central message asked me to send it back. I contacted you on 5, 7 and 13 June. I wanted to know whether you had it, not to hear the departments explain each other.”

The contact extract holds CT00336, CT00337 and CT00338 for those dates. Themes are adviser labels; the longer account is a later synthetic research paraphrase, not an exact transcript of each logged event.

### Service escalation linked to R0852

The retained contact events on 3, 9 and 13 June concern reference/advice issues before the first payment attempt. The later customer research account also discusses a rejected payment, but is **not an additional event row** in the frozen contact extract. Do not assume the three earlier contacts were caused by the rejection on 19 June.

### Store email linked to R0855, 11 June

“We accepted the goods and have the web order. Is £139 within our authority or not? The counter handbook says £150, Finance's email says £100, and the online payment cannot be done at our till. Please confirm the route before we promise a date.”

The email is a source question. It does not establish the final authority decision or prove that all elapsed waiting was caused by the threshold issue.

### Cancellation/evidence account linked to R0853

A dispatch-evidence entry is logged on 4 June; first goods receipt is 13 June. Customer wording says “I already sent proof”. The retained dataset does not include the proof image, a full cancellation assessment or evidence of when a decision maker considered it. Ruth has asked to review the factual evidence and current legal text.

### Partial-order query linked to R0858

Goods amount £39.50; standard delivery paid on the order £4.95; whole_order_return = no. The case does not supply the full basket, actual delivery service or a validated entitlement assessment. Finance queried “delivery amount?” on a reconciliation note. The participant must identify missing facts rather than manufacture an approved rule.

## 7. BE06 — financial and capacity inputs

Finance planning rates: adviser £24/hour; warehouse £20/hour; Finance £32/hour; branch service £22/hour. Rates include an allocation of employment cost and are not supplier invoices or guaranteed cash avoidance. Internal analyst and integration planning rates appear in the systems pack.

The June cohort has 3,473 recorded adviser handling minutes and £90 contact compensation by cutoff. The April cohort has 1,521 minutes and £60 compensation. Different observation maturity and demand mix matter. Recorded active handling excludes queue waiting, unlogged outbound work, store time and warehouse search time.

No validated attrition, dispute-fee, fraud-loss or stock-write-down model is provided. There is no approval to monetise every open requested refund as a loss. Supplier quotes omit some delivery components. Any business case must show which quantities are observed, estimated, missing or dependent on adoption.

## 8. BE07 — records access and outstanding evidence

The coordinator can provide the frozen CSVs and the source excerpts in this repository. The exercise does not contain actual receipts, photographs, payment tokens or personal documents. Requests for such material should be recorded with purpose and the decision affected; the facilitator may confirm that it is unavailable.

The BA has not received a complete legal case review, a full audit sample list, a branch-level transfer dataset, an approved retention schedule, a complete time study or a contracted connector specification. A credible recommendation can recognise those limits and make a conditional decision; it cannot present invented facts as evidence.

Keep the original extracts unchanged. Use stable IDs when citing records. Any new calculation, grouping, model, rule, risk assessment or proposed requirement is the participant's work and belongs in the separate delivery repository.

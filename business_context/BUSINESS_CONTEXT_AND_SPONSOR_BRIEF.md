> **Commission note:** This is historical fictional source evidence. Requests for full lifecycle outputs or pilot delivery are stakeholder ambitions to evaluate. The assessed scope and endpoint are defined in [the current project brief](../project/PROJECT_BRIEF.md). Later pilot evidence is optional and is not participant-executed testing.

# Northbank Home & Style — business context and sponsor initiation brief

**Mettelo Business Analyst Project Studio · MTL-BA-041 · Source pack v2.0**  
**Issued:** 6 July 2026 · **Business snapshot:** 30 June 2026 · **Release:** 1  
**Author:** Helen Ward, Operations Director, with Finance and Trading contributions  
**Classification:** Fictional internal business material. All organisational figures and people are synthetic.

## 1. Organisation and trading model

Northbank Home & Style Ltd is a privately owned UK retailer of homeware, soft furnishings, small electrical appliances and personal-care products. It operates 18 stores in England and Wales, a transactional website and one leased Midlands distribution centre. The business employs 286 permanent colleagues and increases warehouse and service staffing seasonally. Annual sales for the last completed financial year were £34.2 million, including VAT; ecommerce contributed 38%. The trading board expects online sales to grow faster than stores over the next two years.

Customers include households buying everyday home products, customers furnishing a new home and gift buyers. Online purchases can be delivered to a home address or collected from a store. A customer may subsequently take an online purchase to any store, even if that branch does not stock the product. The product mix matters: an unwanted cushion, a faulty kettle, an incorrect item and an opened sealed personal-care product do not necessarily present the same decision. Promotional bundles, partial-order returns and separately charged delivery add further variation. This exercise excludes marketplace sellers and international sales.

Stores have till-based transactions and a branch duty-manager structure. Ecommerce owns the web checkout, customer order history and published help text. Warehouse staff receive postal returns and consolidated store transfers. Customer Service handles calls, email, webchat and central return cases. Finance controls central refund files and provider reconciliation. Store till refunds take a different technical route but appear in the central reporting extract after reconciliation.

The 12-person Customer Service team includes one manager and two team leaders; only eight advisers are normally available simultaneously once training, leave and administration are allowed for. Returns compete with delivery enquiries and order amendments. Four warehouse colleagues rotate between return receiving, inspection and resale preparation; they are not four dedicated returns analysts. Two Finance colleagues process central refund batches alongside other duties. Branch staffing varies; a store manager may also be handling queues and stock deliveries.

## 2. Current operating environment

Northbank introduced online-to-store returns eighteen months ago to improve convenience and encourage repeat visits. No single cross-channel record replaced the existing tools. Store colleagues can see online order information through a lookup screen but cannot authorise a central card refund directly. They record receipt locally, contact Service and consolidate goods for depot transfer. Some teams treat acceptance in store as the start of the returns clock; others use depot receipt, inspection, Finance authorisation or provider submission.

A March promotion increased mixed baskets and cross-channel enquiries. In May, Finance circulated a fraud-control email about approval thresholds. The formal operations handbook was not reissued. At the same time, warehouse agency cover was reduced and Ecommerce refreshed the help page. Leadership does not yet know whether those events explain the deterioration, whether problems were present earlier, or whether reporting changes made them more visible.

The trading calendar adds pressure. Autumn promotional stock arrives in September. The sponsor wants a limited operational pilot on 12 October, before a configuration freeze on 1 November. Peak trading is a reason to resolve uncertainty; it is not permission to remove controls or mislead customers about refunds.

## 3. System and information environment at appointment

OrderHub is the online order platform. TillPoint records store sales and store-originated refunds. ServiceDesk holds customer contacts and central return cases. DepotSheet is a controlled-access shared workbook for receipt and inspection entries. FinancePay imports approved refund batches and records provider acknowledgements. Management combines exports into a reporting workbook.

The business has no evidence that every displayed status has the same meaning across these products. A ServiceDesk field labelled “refunded” can be selected by an adviser. A FinancePay acknowledgement proves a provider accepted an instruction for processing; it does not itself establish that the customer received the funds. Some store parcels use an order number without a return reference. IT believes existing tools may support additional queue and status configuration, but has not assessed effort or shown the capability with representative exceptions.

These are starting facts and claims, not a completed current-state model. The BA must establish authoritative events, owners, hand-offs and exceptions from later sources.

## 4. Trigger for the engagement

On 29 June the board reviewed three escalations: a web purchase accepted in a branch but described as not received by Service; a customer shown “refund sent” after a provider rejection; and an online cancellation where staff disagreed about the evidence needed before releasing payment. The board did not determine whether a legal breach had occurred. It requested a cross-functional investigation and an investment decision.

Helen Ward has sponsored a new returns platform in the initial capital plan. She believes a single customer status view would reduce avoidable contacts. Finance has challenged the evidence for the investment; the June completion indicator looks faster while unresolved cases and contact demand have grown. Warehouse considers staffing and inconsistent identifiers more important than a portal. Stores question why their inspection is repeated. Compliance is concerned about applying one policy clock to different types of return.

The project is therefore commissioned to support a decision, not to ratify a purchase. No vendor has been selected and no requirements baseline exists.

## 5. Management information supplied at initiation

The following is the **existing board extract**, reproduced from the frozen synthetic cohort records. Each row groups requests by the month first raised, with all observed outcomes cut off at 30 June. It is not a month-of-activity report. April cases have had longer to progress than June cases.

| Request cohort | Requests | Requested goods refunds, GBP | Cases with at least one accepted provider instruction | Cases without an accepted instruction at cutoff | Linked contact events at cutoff | Formal complaint events |
|---|---:|---:|---:|---:|---:|---:|
| April 2026 | 400 | 47,630.15 | 375 | 25 | 136 | 10 |
| May 2026 | 450 | 59,390.26 | 425 | 25 | 199 | 17 |
| June 2026 | 550 | 63,988.15 | 329 | 221 | 295 | 24 |

“Without an accepted instruction” includes several different situations; it is not automatically an overdue liability or a service failure. Goods may not have arrived, a goodwill request may have been declined, a policy query may remain open, or a payment may have failed. Formal complaints are event records and can concern a return already represented in another contact. Neither column is a count of unique customers.

The board workbook also shows mean calendar days from Finance authorisation to first accepted provider instruction: April 2.5; May 2.2; June 1.9. It excludes cases with no accepted instruction. Helen has previously described this as “refund speed”, while Customer Service measures from the customer's original request. No customer-receipt performance promise can be inferred from the authorisation indicator.

The later operational release will let the participant reproduce these source totals and examine the limitations. No analysis of root cause or recommended performance definition has been approved.

## 6. Impact and the cost of doing nothing

June-cohort contact records already contain 3,473 adviser handling minutes at the cutoff, compared with 1,521 for the April cohort. Finance uses £24 per adviser hour as a planning assumption for loaded service capacity; this is not cash that disappears automatically when call demand falls. The June records contain £90 in discretionary contact compensation, excluding the refund itself. They do not include card dispute fees, lost future purchases, outbound calls not logged in ServiceDesk, store time or the opportunity cost of warehouse congestion.

The customer impact is wider than the arithmetic: repeated explanations, inconsistent eligibility advice, uncertainty about where goods are held and difficulty distinguishing payment submission from receipt. Staff describe customers arriving at a store with screenshots that conflict with the adviser screen. Service quality can affect trust, but no attributable churn estimate has been established.

If nothing changes, the organisation could enter peak trading with larger unresolved queues, more manual reconciliation and an inconsistent customer promise. A poorly chosen replacement could also consume scarce delivery capacity, create another source of conflicting statuses and leave process or policy issues intact. Finance wants both risks considered. The BA is not asked to assert that doing nothing will cost a particular amount without evidence.

## 7. Sponsor brief — commissioned work

**Sponsor:** Helen Ward, Operations Director; reports to the Managing Director and chairs the weekly operational change group. Helen can recommend investment and approve the analysis scope. The board approves capital commitments; Finance and the relevant control owners retain their normal authorities.

**Reason for initiation:** establish a credible explanation of the service issues, agree the change needed, and choose an affordable intervention before the autumn delivery window closes.

**Sponsor's current understanding:** “Customers cannot see one reliable status and our teams repeat work. I think a central workflow product will give us control. I do not know how much of the delay is inspection, policy interpretation, an identification problem, payment failures or simply the wrong measure.”

**Desired outcomes, subject to validation:**

- Customers receive accurate, comprehensible progress information and know the next action.
- Refund handling meets applicable obligations and the agreed customer promise for each relevant case type.
- Staff can identify ownership and unresolved exceptions without recreating the case.
- Finance can reconcile approved amounts and provider outcomes with auditable evidence.
- Operational improvements remain usable across busy branches, Service and Warehouse.
- Any investment has an explicit cost, adoption assumption, owner and evaluation method.

Helen's proposed service ambition is for 90% of **authorised central refunds** to reach an accepted provider instruction within two working days. Aisha considers that too narrow to represent customer experience. Priya questions what should count as an authorisation when evidence is disputed. The target is a sponsor proposal, not an approved business requirement or a legal deadline. The BA must bring a proposed measurement set and definitions for stakeholder agreement.

**Executive concerns:** missed peak readiness; repeated fraud or duplicate payment; misleading web wording; disruption to store trading; an unaffordable recurring licence; and a superficially successful pilot that transfers work to another team.

**Initial funding assumptions:** £80,000 one-off including analysis, configuration, integration, migration, testing and internal backfill; annual incremental operating ceiling £15,000. Amounts exclude recoverable VAT. £8,000 of the one-off envelope is already committed to analysis/support, leaving £72,000 uncommitted at appointment. Do not add the £8,000 again when costing options. Existing business-as-usual salaries are not incremental cash costs unless backfill or additional capacity is requested.

**Schedule:** eight-week analysis engagement from 6 July to 28 August 2026. Sponsor decision on the preferred approach is expected at the final playback, with earlier scope and priority decisions as evidence emerges. The desired operational pilot is 12 October; November freeze remains. The August supplier experiment supplied later is an isolated synthetic demonstration, not the October operational pilot.

**Who Helen initially wants involved:** Service, Warehouse, Finance, Ecommerce, Store Operations, IT and Compliance. Helen asks Jo Evans to represent branches but acknowledges that one store cannot speak for all operating conditions. Customer voices, branch colleagues outside Jo's store, reconciliation staff, the payment provider and information governance may require further involvement. Their approval must not be assumed.

## 8. Commissioned perimeter and exclusions

The initial investigation covers UK consumer goods refund requests from first contact through goods/evidence handling, eligibility/authority decisions, payment instruction, rejection follow-up and customer confirmation. It includes online purchases returned by post or to a store and store purchases returned in store. It includes exception handling, data/status ownership, reporting and operational adoption.

It does not commission international sales, business-to-business contracts, marketplace disputes, price changes, full warehouse redesign, replacement of the payment provider or a new ecommerce platform. Repair/replacement enquiries are relevant when distinguishing the appropriate customer route, but designing the entire repair supply chain is outside the initial funded perimeter. Any boundary change needs a recorded sponsor decision. This is the sponsor's initial perimeter, not the participant's completed scope analysis.

## 9. Constraints, risks, assumptions and dependencies

The nightly OrderHub export is available; a real-time write-back interface is not confirmed. Store staffing cannot be assumed to increase. Warehouse agency cover is expected to reduce by two shared shifts per week in August. Staff can normally attend one 45-minute workshop per week. Provider settlement timing is not fully controlled by Northbank.

The sponsor assumes that existing order identifiers can link most records, that an October pilot can be contained to a small group and that the annual ceiling includes support. None is yet proven. Dependencies include supplier interface confirmation, a legally reviewed customer promise, Finance reconciliation approval, branch participation, role/access review and time for training and exception testing.

Known risk observations include uncontrolled policy copies, disagreement over when receipt occurs, missing references, ambiguous payment labels and insufficient evidence of customer settlement. These are management concerns, not a completed RAID log. Participants must investigate likelihood, impact, ownership and responses themselves.

## 10. The decisions leadership needs

At the end of the engagement Helen expects a recommendation on whether to configure current tools, redesign working practices, add a limited workflow capability, purchase a replacement, sequence interventions or defer part of the change. She expects a defensible cost range, scope, priorities, implementation dependencies, readiness conditions and benefits evaluation proposal.

The BA must make uncertainty visible. How much demand is avoidable? Which clocks matter for each purpose? Which decisions require different evidence or authority? Which system claims survive an exception-based demonstration? What can be achieved before peak without shifting risk to customers or colleagues? What information is still missing, and what decision can reasonably be made without it?

No document in this pack supplies an agreed problem statement, stakeholder assessment, process map, requirements catalogue or preferred solution. Those are the participant's work.

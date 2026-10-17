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


## Business need for this commission

Returns move through stores, warehouses, customer service and Finance with inconsistent evidence, policy interpretation and hand-offs. Customers chase refunds while staff cannot always distinguish an authorised case, an accepted payment instruction and money received by the customer. Management sees delay but does not yet know which causes can be removed through working practices and controls.

A process improvement decision must come before a system purchase. A new portal could simply make an unclear process more visible, while staff effort and unresolved payment exceptions remain. The business needs an evidence-backed proposal for how work and accountability should change.

## Illustrative business situation to investigate

A customer starts a return online or takes goods to a store. A colleague captures the request; another team may receive and inspect the goods; an authorised person decides the refund; Finance passes an instruction to the payment provider. If a reference is missing, an instruction is rejected or the policy route is disputed, the case may return to an earlier queue. Customer Service sees a complaint but may not see a confirmed settlement. This is a business situation to investigate, not an approved process map.

This is a source scenario. Your team must analyse it; it is not an approved process, detailed use case or designed solution.

## Sponsor commission and authority

Helen, the project sponsor commissions your team as process improvement business analysts. The decision is: **Which operational changes should Northbank fund, in what order and under whose ownership, to reduce avoidable delay and inconsistent decisions?**

The requested handover is: **A process improvement recommendation, proportionate business case and operational transition/benefits plan for leadership decision.**

The sponsor wants faster refunds, Finance wants reliable reconciliation, stores need workable delegation, and warehouse colleagues need manageable inspection work. A faster step is not automatically a better end-to-end outcome if it increases errors or shifts work to another team.

The sponsor can request analysis but cannot substitute for Finance, policy, legal, security and funding owners. Identify material approvals and unknowns without fabricating named reviewers or sign-off.

## Scope and exclusions

**Included:** Store and online return-to-refund work, policy routing, authorisation, inspection, payment exceptions, reconciliation and customer status communication. Proposed systems changes may be dependencies, but the core work is operating-process improvement.

**Outside this assignment:** No replacement-system FRD, detailed interface specification, agile product backlog, executable system or full system UAT portfolio is required. Participants do not issue legal determinations or process real refunds.

## Constraints and evidence limitations

The initial one-off planning envelope is £80,000, including £8,000 committed; the annual incremental ceiling is £15,000. Later released funding evidence may constrain the recommendation. Include internal effort, exclusions and recurring costs; a quote is not a complete business case.

The learning commission lasts 6 cohort weeks. Original dates in operational records remain source history; later operational ambitions do not extend the assessed scope. Staff availability is limited: plan proportionate elicitation using supplied interviews and record follow-up questions when real access is unavailable.

The dataset is constructed, observed at its stated cutoff and incomplete for some business questions. An absent event is not always proof an event did not happen. Do not claim representative research, causality, approved targets or realised outcomes merely from these records. Use [the data guide](../evidence/DATA_GUIDE.md) and [source provenance](../reference/OFFICIAL_REFERENCES_AND_SOURCE_PROVENANCE.md).

## How the evidence supports the work

| Evidence | Analytical purpose | Relevant tasks |
|---|---|---|
| Returns, payment attempts and contacts | Separate cases, transaction attempts and chasing activity; establish reproducible baseline measures. | P1–P3 |
| Interviews, forms and business evidence | Understand actual hand-offs, disagreement and exceptions before modelling improvements. | P2–P4 |
| Policies and technology context | Investigate delegation and payment constraints without assuming a new system is the answer. | P3–P5 |
| Process investigation supplement | Challenge clocks, training capacity and operational ownership. | P2–P6 |
| Challenge notices | Revise affordability, policy and implementation dependencies within the process recommendation. | P5–P7 |

## What leadership needs to receive

Leadership can see which delays and policy gaps are evidenced, compare credible interventions and decide on accountable operational changes. Proposed outcome measures must define their clocks, denominators, owners and limitations; no achieved saving or improvement is supplied.

| Task | Required handover content | Assessment weight |
|---|---|---|
| P1 | Problem statement; scope; baseline workbook with calculations, cohort/cutoff, source references and limitations. | 20% |
| P2 | Readable AS-IS swimlane maps for store/online routes; root-cause analysis with evidence and untested hypotheses. | 20% |
| P3 | Policy clarification log; proposed operational controls; disputed thresholds and named decision roles, with unresolved approvals. | 15% |
| P4 | TO-BE maps; operational procedure outline; explanation of changes, hand-offs, exceptions and responsibilities. | 15% |
| P5 | At least three credible options; cost assumptions and sensitivity; recommendation within released constraints. | 15% |
| P6 | Role-level change impact assessment; adoption/training sequence; benefits definitions, owners and measurement plan. | 10% |
| P7 | Sponsor decision paper; playback of no more than ten slides or equivalent; indexed recommendation and outstanding decisions. | 5% |

Use [the task specification](../project/TASKS_DELIVERABLES_AND_ACCEPTANCE_CRITERIA.md) for the four acceptance criteria per task and [the submission checklist](../submission/DELIVERABLES_CHECKLIST.md) for the exact handover package. These define the commission; historical stakeholder ambitions are inputs to evaluate, not extra mandatory portfolios.

No preferred solution or completed learner artefacts are provided.

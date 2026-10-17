# Operational evidence — extraction guide and dictionary

**Mettelo Business Analyst Project Studio · MTL-BA-041 · Stage 3**  
**Extract frozen:** 30 June 2026, 18:00 UK · **Issued to BA:** 20 July  
All records were generated for this simulation. They are not anonymised real customer data.

## 1. Population and sampling

operational_data.csv contains all **1,400 synthetic refund requests in the defined training population** first raised in April (400), May (450) or June (550). It is a constructed population for the simulation, not a sample to extrapolate to Northbank's entire sales base. Requests include online purchases returned by post or to store and store purchases returned to store. Exchanges that never became refund requests, international sales and other excluded business lines are absent.

payment_attempts.csv contains **1,223 observed attempts** linked to those returns through the cutoff. A return may have no attempt, an accepted attempt, a rejected attempt followed by a replacement, or a blocked duplicate. customer_contact_events.csv contains **630 observed inbound contact events**, not 630 unique customers.

The management table groups by request cohort and observes outcomes through the common cutoff. It does not count all events occurring in each calendar month. Later cohorts have had less time to progress. Unobserved later dates remain blank. Do not treat blanks as zero days or infer that a case never completes.

## 2. Operational data fields

| Field | Source meaning and important limitation |
|---|---|
| return_id | Unique central/reconciled return reference; one row per refund request |
| order_id | Synthetic order reference, not a person identifier; this frozen training population has one included request per order |
| purchase_channel | online or store; describes original purchase, not where goods were returned |
| return_route | post or store; a route, not a full process |
| receiving_site | First receiving branch S01–S18 or warehouse WH01; does not describe every later physical movement |
| product_category | Intake product grouping; not sufficient for legal applicability |
| reported_reason | Customer/intake label; not a validated finding of fault or entitlement |
| order_delivered_date | Recorded delivery/possession date used for this exercise; store records use the sale/handover date |
| request_date | Date the included central refund request was first recorded; earlier informal contact is not established |
| dispatch_proof_logged_date | Date evidence of dispatch was logged, if present; content and legal sufficiency are not verified by this field |
| first_goods_received_date | First observed Northbank custody date, including branch acceptance; not necessarily depot receipt |
| inspection_recorded_date | Date inspection was recorded; may be later than physical work; evidence detail is elsewhere or missing |
| finance_authorised_date | Recorded release authorisation date; does not independently prove appropriate authority or eligibility |
| refund_requested_gbp | Goods refund requested, gross GBP; not automatically an approved liability, payment or benefit |
| standard_delivery_paid_gbp | Original standard delivery paid on the order; no conclusion about entitlement to refund it is supplied |
| whole_order_return | yes/no intake field; validate basket facts for any delivery-charge decision |
| opened_seal | yes/no/not_recorded for relevant category, otherwise not_applicable; not a legal exception decision |
| source_status | Reconciled snapshot label; not an approved future lifecycle |
| receipt_link_method | return_id or manual_match; states how source records were linked, not whether the match was correct |

Dates are ISO YYYY-MM-DD with calendar-day precision. There is no event time-of-day, timezone ordering within a day, full holiday calendar, basket-level dataset, complete eligibility assessment, photographic evidence or full physical transport log. The later sources discuss selected case history. The participant must say which questions remain unanswered.

## 3. Payment attempt fields and safe interpretation

attempt_id is unique. return_id links to operational_data. attempt_date records submission; amount_gbp is the attempted goods amount. provider_result is accepted, rejected or blocked. accepted means accepted for processing; rejected means the instruction was rejected; blocked means a duplicate-reference guard prevented that attempt proceeding.

replaces_attempt_id points to an earlier rejected attempt for the same return where a retry is explicitly linked. A separate blocked duplicate need not have a replacement link. Do not sum every attempt as money paid or count retries as new returns.

settlement_confirmed_date is populated only where the reconciliation source contains a confirmation by cutoff. A blank is unverified settlement, not proof of non-payment. This field is not a customer's bank statement. It is distinct from the date an adviser selected a ServiceDesk label.

The R0852 replacement and R0857 blocked duplicate are deliberately retained source exceptions. They do not provide a full confirmed duplicate-loss rate or demonstrate that Northbank's controls are generally adequate.

## 4. Contact event fields

contact_id is unique. return_id links the event to a case. contact_date is the logged event date. channel is phone/email/webchat. contact_type is status_enquiry or repeat_contact within the retained central-contact sequence. theme is the adviser's primary label; it may not capture every issue raised. handling_minutes is recorded active handling time, excluding queue time and work not logged against the event.

formal_complaint is an adviser-applied yes/no flag, not an independent assessment of regulatory classification or unique dissatisfied customers. goodwill_compensation_gbp is an additional discretionary amount recorded for that contact, separate from the goods refund request. Sum it only for the question and population you intend.

One return may have several contacts. A contact after a settlement confirmation does not itself prove failure: its subject, timing or the customer's understanding may differ. No customer identifier is provided, so unique-person metrics cannot be derived.

## 5. Reporting basis and financial assumptions

The Stage 1 board figures are published source information that can be reproduced from the frozen records. They are not model answers to the BA analysis. Reproduce the grouping, cutoff and accepted-case definition before comparing them with another measure. A cohort's case counts and event counts are different units.

Finance's planning rate for adviser effort is £24/hour; warehouse £20/hour; Finance £32/hour; branch service £22/hour. These rates are indicative loaded capacity values, not automatic cash savings. Incremental backfill, actual supplier charges and avoided cost need separate evidence. No reliable attributable churn, fraud-loss or card-dispute cost population is provided.

## 6. Deliberate information limitations

The frozen extracts are structurally consistent, but business information is incomplete. Exact event times, verified entitlement, complete authority evidence and every local workaround are absent. Definitions differ in the source systems. The coordinator's reconciliation does not prove live interoperability or remove the need to investigate source provenance.

Do not “clean” away failed attempts, open cases or repeated contacts merely because they complicate analysis. Keep raw sources unchanged in your separate delivery repository; document transformations, assumptions and exclusions. Identify the difference between a data-quality issue, an unobserved event and a genuine business exception.

## 7. Later pilot dataset

pilot_observations.csv is **Stage 6 material**, not a continuation of the April–June population. It contains 96 operator observations: 48 baseline replays and 48 prototype trials, paired through paired_case_id. source_return_id links to historical synthetic case facts, not a new real return.

An operator task time is not end-to-end refund duration. Ratings are ordinal; visibility flags record what the observer could see in that trial, not validated acceptance. Repeated use of known cases, assistance, order effects and limited operator coverage affect interpretation. Read the delivery/pilot pack at release before using those fields.

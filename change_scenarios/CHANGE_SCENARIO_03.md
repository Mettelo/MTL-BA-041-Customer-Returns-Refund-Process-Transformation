# Change notice 03 — interface constraints before the pilot

**Mettelo Business Analyst Project Studio · MTL-BA-041 · Stage 5C**  
**Raised:** Friday 7 August 2026, 11:00 · **Raised by:** Oliver King, IT Manager  
**Evidence:** written supplier interface response and payment-adapter estimate  
**Decision forum:** 10 August · Release after the participant records the policy notice response.

## 1. What prompted the update

Oliver asked the vendors to confirm the integrations used in the original portal demonstration. The demonstration had immediate seeded responses and did not use Northbank's production products. The written response is more limited than the trading team assumed.

This notice does not prescribe a future architecture. It gives confirmed delivery constraints for options that depend on those interfaces.

## 2. Supplier response — OrderHub

“Under the present contract, Northbank has the existing nightly read-only export. Return-status write-back requires an interface extension and supplier release slot. Earliest available release is **16 November 2026**, subject to specification, testing and contract agreement. We cannot commit to real-time write-back for the **12 October** operational pilot.”

The nightly file remains available at 02:00 UK. Its continued availability does not establish that every downstream record is fresh, correctly matched or suitable for a customer promise. A display may need to explain what is known and when it was last updated; the participant must determine and validate the actual need.

The £18,000 connector figure in FlowReturn's earlier commercial input was an **indicative allowance**, not a committed October delivery slot. It is not a second separate £18,000 charge to add automatically.

## 3. Payment adapter response

“The standard portal package does not include automatic provider-rejection events. A daily response-file adapter is estimated at **£4,500 one-off plus £1,500 annual support**, with six weeks from approved scope and access. Real-time rejection-event integration has no committed date before peak.”

These are new excluded-cost estimates, not an approved purchase. The proposed daily adapter would still need a business owner, reconciliation and review of failed/replayed files. FinancePay's existing response files remain available for a controlled manual or other approved handling route; this notice does not authorise ignoring rejections.

## 4. Why this matters to the present decisions

Any baseline relying on immediate OrderHub write-back or real-time provider-rejection events now rests on an unsupported pre-pilot assumption. An approach using current tools or nightly files may be less affected, but it must still address data meaning, communication, error handling and operational effort.

No statement in this notice says the portal should be abandoned or that current tools are sufficient. The participant must assess the value, feasibility and risk of their own alternatives under the confirmed constraints.

## 5. Recorded stakeholder reaction

**Helen:** “I am not moving the desired October pilot just to preserve an integration assumption. Bring me a narrower credible pilot, another sequence or a clear case that the readiness conditions cannot be met.”

**Ben:** “My team told leadership the demo looked instant. We need to correct that expectation. I do not want a customer screen silently showing yesterday's status as current.”

**Aisha:** “A daily queue could still help if advisers know what is stale and who acts on a rejection. An attractive 'refund sent' message without the exception route would make our job worse.”

**Priya:** “Add the excluded costs and support to the relevant option. Show me how we reconcile after a missed response file. Do not imply that the subscription already includes this.”

**Jo:** “Please explain what my counter colleagues will do when their receipt is newer than the central view.”

**Oliver:** “A workaround is still a process requiring capacity, control and testing. I can assess it once the priorities and decisions are clear.”

## 6. Constraints retained

Funding remains £56,000 total one-off including the £8,000 commitment, and £15,000 annual incremental cost. The desired operational pilot is 12 October, configuration freeze 1 November. No policy issue from Notice 02 is waived. Supplier and internal-resource estimates still exclude any items explicitly excluded in the original sources.

November delivery cannot be described as an October capability. A solution may be sequenced, but it must state what exists at each point, what work remains and what approval/readiness evidence is needed.

## 7. Decision required from the change group

The BA should bring a reasoned scope, sequencing or funding recommendation for 10 August, explaining the effect on customer/service objectives, affected needs and priorities, controls, systems/data dependencies, transition effort, tests, operational ownership and benefits assumptions. Retain traceability to the earlier baseline.

The sponsor can choose to escalate, narrow, sequence or defer; the BA must not silently accept an unsafe assumption to meet a date. A readiness recommendation can challenge the desired pilot if evidence is insufficient. No revised design, requirements catalogue, future process or approved go-live decision is included here.

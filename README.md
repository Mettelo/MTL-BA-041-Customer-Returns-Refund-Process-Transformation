# MTL-BA-041 — Customer Returns & Refund Process Transformation

## Start with the tasks and required deliverables

**Project type:** Business process improvement and operational analysis. Customer returns and refund handling across stores, Service, Warehouse, Finance and Ecommerce.

Open [What you must do, deliver and demonstrate](project/TASKS_DELIVERABLES_AND_ACCEPTANCE_CRITERIA.md) before starting. It defines **D01–D12**, exact output paths, timing, project-specific coverage and **48 assignment acceptance checks**. Start at D01; D04 requires your own requirements and solution acceptance criteria, and D09 requires tests derived from them.

The change notices are later scope/requirements constraints handled in D08. They do not turn this project into an organisational change-management assignment. Produce all work in your separate delivery repository; no answers belong in this master.


**Mettelo Business Analyst Project Studio**  
**Client:** Northbank Home & Style Ltd — fictional UK retailer  
**Role:** Business Analyst · **Engagement:** eight weeks, 6 July–28 August 2026  
**Resource pack:** v2.0 · **Status:** substantial replacement prepared for Mettelo review

You are joining a cross-functional change engagement at a retailer with 18 stores, an ecommerce operation and a shared distribution centre. Customers receive inconsistent refund updates; teams disagree about evidence, ownership and the point at which a refund becomes ready. Leadership suspects a new returns system is needed. Your job is to investigate the business need and support an investment and readiness decision.

This is a BA simulation, with incomplete source information and competing stakeholder accounts. It is not a dashboard assignment or a specification to implement. All organisational data, people, correspondence and experiment records are synthetic. The official legal references are genuine and separately identified.

## Start here

1. Read the [business context and sponsor brief](business_context/BUSINESS_CONTEXT_AND_SPONSOR_BRIEF.md).
2. Read the [participant brief](project/PROJECT_BRIEF.md), [delivery guide](project/DELIVERY_GUIDE.md) and [timeline](project/PROJECT_TIMELINE.md).
3. Set up your **own separate delivery repository** using the [Mettelo submission guidelines](submission/SUBMISSION_GUIDELINES.md).
4. Record your initial questions, assumptions and scope interpretation before opening later evidence.
5. Work through the release gates, saving a dated baseline before each new change notice.

The [assessment criteria](project/ASSESSMENT_CRITERIA.md) reward reasoning, validation, traceability and decisions. Document quantity alone earns no marks.

## How evidence arrives

| Stage | What Mettelo supplies | What you do |
|---|---|---|
| 1 — Initiation | Business context, sponsor brief, commissioning instructions | Establish your understanding, boundaries, assumptions and discovery plan |
| 2 — Discovery and elicitation | One consolidated stakeholder/interview pack | Analyse perspectives, plan follow-ups and validate ambiguity |
| 3 — Current-state investigation | Linked operational extracts, business evidence, existing forms, policy and system sources | Reconstruct the current situation and investigate causes, exceptions and measures |
| 4 — Requirements and future state | No answer pack; facilitator responses only where supported | Develop your own needs, rules, models, options and testable priorities |
| 5 — Constraint events | Three detailed notices released in order | Assess each change against your saved baseline and request decisions |
| 6 — Delivery and UAT | Supplier experiment notes and 96 observation records | Define independent tests, judge evidence and assess readiness |
| 7 — Recommendation and playback | Executive challenge session | Make a qualified recommendation, explain residual uncertainty and propose evaluation |

See the [release manifest](project/RELEASE_MANIFEST.csv) for exact file assignments. Stage numbers are lifecycle stages, not a promise of a new dataset every week. Stages 4 and 7 primarily involve your own synthesis and stakeholder playback.

**This is a public master resource repository.** It contains all source stages for facilitator inspection. Public GitHub folders and branches cannot hide later evidence. For a controlled cohort, Mettelo should distribute only the current stage's files in a private learner space and retain the later files. Self-directed learners should stop at each gate before reading ahead. Downloadable stage packs support distribution but do not enforce secrecy while this source library is public.

## What the evidence contains

The June snapshot covers **1,400 refund requests** first raised in April–June, linked to **1,223 payment attempts** and **630 customer contact events**. It includes open cases, repeated contacts and failed/retried provider instructions. A [data guide](evidence/DATA_GUIDE.md) explains population, timing, units, limitations and joins. Raw extracts support analysis; they are not an agreed current-state model.

The [stakeholder pack](stakeholders/STAKEHOLDER_AND_ELICITATION_PACK.md) brings together sponsor, frontline, branch, warehouse, Finance, IT, Ecommerce, Compliance and customer perspectives. It intentionally preserves disagreement. A senior role's statement is not automatically a requirement or a policy approval.

Later pilot material represents a supplier's disputed experiment with synthetic replay records. It is not the correct solution and need not match the approach you recommend. Supplier claims, quotes and demonstrations require challenge.

## What you must produce

Build a coherent evidence portfolio covering the business problem and scope; your stakeholder analysis and elicitation record; current and proposed processes; reasoned cause analysis; business, functional, non-functional and transition requirements; business rules and exceptions; appropriate use cases or user stories with acceptance criteria; prioritisation; options and costs; requirements traceability; RAID and change impacts; UAT and readiness; recommendation and benefits evaluation.

Choose a practical document structure. Requirements and tests may live in linked registers rather than one file per artefact. Make it possible to follow a material need from its source through a decision, design implication, test and intended benefit. Do not claim approvals you did not obtain.

## What to avoid assuming

A portal may improve visibility without changing refund eligibility, inspection capacity or payment settlement. A faster completed-case average may omit unresolved demand. A provider acknowledgement is not necessarily receipt of money by a customer. Different return reasons can involve different legal considerations. Staff recollections, uncontrolled emails and signed policy versions may conflict. Investigate rather than silently resolving these points.

The source pack does not include completed stakeholder matrices, process maps, root-cause findings, requirements, user stories, decision tables, traceability matrices, UAT scripts or an options recommendation.

## Source library

- [Business context and sponsor brief](business_context/BUSINESS_CONTEXT_AND_SPONSOR_BRIEF.md): organisation, impact, initial investment assumptions and decision sought.
- [Stakeholder and elicitation pack](stakeholders/STAKEHOLDER_AND_ELICITATION_PACK.md): substantial interviews and workshop extracts.
- [Business evidence pack](evidence/BUSINESS_EVIDENCE_PACK.md): observations, audit extracts, communications and cost inputs.
- [Data guide](evidence/DATA_GUIDE.md): definitions and limitations for the linked CSV evidence.
- [Existing forms and communications](evidence/forms/EXISTING_FORMS_AND_COMMUNICATIONS.md): current blank forms and conflicting message text.
- [Policy and business rules sources](policies/POLICY_AND_BUSINESS_RULES_PACK.md): existing fictional policies and disputed interpretations.
- [Current systems and technology context](systems/CURRENT_SYSTEMS_AND_TECHNOLOGY_CONTEXT.md): capability claims, constraints and raw commercial inputs.
- [Official references and provenance](reference/OFFICIAL_REFERENCES_AND_SOURCE_PROVENANCE.md): external links, applicability boundaries and workflow precedents.
- [Delivery and pilot evidence](evidence/DELIVERY_AND_PILOT_EVIDENCE_PACK.md): later-stage material; open only at Stage 6.
- [Submission guidelines](submission/SUBMISSION_GUIDELINES.md): separate-repository workflow and final handover.

## GitHub and submission

Keep this Mettelo master repository as the brief/resource library. **Never push participant answers or answer pull requests here.** Create a distinct repository named `MTL-BA-041-<team-name>`, preferably under Mettelo where cohort access permits. Individual participants use an agreed individual identifier in place of team name.

Use issues for material work, branches for substantial changes, meaningful commits and pull requests for material merges. Keep individual contribution evidence. Verify that the designated Mettelo reviewers can inspect the repository and history. Complete your own final submission record, create `v1.0-mettelo-submission` and submit your delivery repository URL through the cohort route supplied by Mettelo. Do not email project files or invent a submission portal.

Mark your portfolio **“Mettelo simulated Business Analyst engagement”**. The exercise can demonstrate analysis and decision-making; it is not evidence of employment by Northbank or a real client implementation.

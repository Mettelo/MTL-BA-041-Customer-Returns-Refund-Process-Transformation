# Evidence dictionary and extraction notes

Transaction sample: 12 hand-selected cases requested in June, snapshot 30 June 2026 at 18:00 UK. One row per return; IDs are unique. Blank dates mean event not observed by cutoff, not zero duration. Dates are calendar dates; no time-of-day precision. Received means goods first accepted by store or warehouse. Inspection may be later at warehouse. Submitted is sent to provider, not money received. provider_failed retains submission date. Amount is requested gross refund in GBP.
Complaints: one row per contact/complaint record; R004 has two records, so complaint counts are not unique customers. repeat_contacts is the adviser's count of earlier contacts, not additive across rows.
Monthly performance: full monthly dashboard population, not derivable from the 12 cases. Means include completed provider submissions only and exclude unresolved cases. No distribution or raw population was supplied; do not calculate a population percentile from means.
Issues: reported symptoms, not confirmed root causes. All case IDs refer to transaction sample. Working-day calculations need a declared UK holiday calendar and event semantics.

---
Mettelo Business Analyst Project Studio | MTL-BA-041 | Fictional simulation source | Release 3

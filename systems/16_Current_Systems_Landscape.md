# Current systems — IT note, 13 July

OrderHub holds online order IDs. TillPoint holds store receipts. DepotSheet is a shared workbook with parcel and inspection notes. ServiceDesk holds contacts and return IDs. FinancePay imports a CSV and returns provider submission or rejection references.
OrderHub exports at 02:00 UK time; it has no contracted write-back API. TillPoint exports branch batches at close. Store return IDs are free text. ServiceDesk cannot display provider rejection events today.
IT owns integrations; Finance owns reconciliation. A failed file import must be resubmitted manually. 'Paid' on ServiceDesk is an adviser-selected label, not a bank settlement confirmation.

---
Mettelo Business Analyst Project Studio | MTL-BA-041 | Fictional simulation source | Release 3

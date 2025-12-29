# Configuration Mapping

## Objective
Map business requirements and solution design into Salesforce configuration decisions, ensuring clarity before implementation.

---

## Sales Configuration

### Lead Management
- Salesforce Object: Lead
- Purpose: Track unqualified prospects from inbound and outbound channels
- Key Configuration Decisions:
  - Leads will be owned by Sales reps
  - Lead status will indicate qualification progress
  - Leads will be converted once qualified

### Account & Contact Setup
- Salesforce Objects: Account, Contact
- Purpose: Represent customers and stakeholders after lead qualification
- Key Configuration Decisions:
  - One Account can have multiple Contacts
  - Accounts act as the primary reporting entity

---

## Support Configuration

### Case Management
- Salesforce Object: Case
- Purpose: Track customer issues and service requests
- Key Configuration Decisions:
  - Cases must always be linked to an Account
  - Each Case is associated with a Contact
  - Case priority will drive SLA tracking

---

## Reporting Configuration

### Executive Reporting
- Primary Reporting Object: Account
- Supporting Objects: Case, Lead
- Reporting Outcomes:
  - Visibility into sales pipeline by Account
  - SLA performance by customer
  - Support workload trends

---

## Design Guardrails
- Avoiding unnecessary customization
- Preferring standard Salesforce objects over custom objects
- Optimized for reporting clarity and user adoption

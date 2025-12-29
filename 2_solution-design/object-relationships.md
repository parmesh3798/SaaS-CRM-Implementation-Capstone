# Object Relationships

## Overview
This document defines how core CRM entities relate to each other to support sales operations, customer support, and reporting needs.

## Lead to Account & Contact
Leads represent unqualified prospects.
Once qualified by Sales, a Lead is converted into:
- An Account (company)
- A Contact (person)

This separation ensures clean reporting between prospects and customers.

## Account to Contact
An Account can have multiple Contacts.
This reflects real-world B2B relationships where multiple individuals work at the same company.

## Account to Case
Cases are always associated with an Account.
This allows support teams to view customer issues in the context of the overall customer relationship.

## Contact to Case
Each Case is linked to a Contact.
This identifies the individual who reported the issue and enables personalized support.

## Design Considerations
- Accounts act as the central reporting entity
- Relationships are kept simple to avoid adoption issues
- Structure supports both operational and executive reporting

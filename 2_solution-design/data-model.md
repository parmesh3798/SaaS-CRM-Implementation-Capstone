# Data Model Design

## Objective
Design a simple, scalable data model that supports sales tracking, customer support, and executive reporting needs identified during discovery.

## Core Entities

### Account
Represents a company that the business sells to.
Accounts serve as the primary parent entity for all customer-related data.

### Contact
Represents an individual working at an Account.
Contacts are used for sales communication and support interactions.

### Lead
Represents a potential customer who has shown interest but is not yet qualified.
Leads are converted into Accounts and Contacts once qualified by Sales.

### Case
Represents a customer issue or support request.
Cases are used by the Support team to track resolution and SLA performance.

## Design Principles
- Keep the data model simple to encourage adoption
- Avoid duplicating information across entities
- Design for current needs, with room to scale later

## Out of Scope (For Now)
- Advanced custom objects
- Deep integrations
- Complex hierarchy models

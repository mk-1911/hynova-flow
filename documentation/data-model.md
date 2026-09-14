# Data Model

HYNOVA Flow uses a structured relational-style data model
implemented within Microsoft Excel tables.

The major entities are:

- Leads
- Clients
- Projects
- Tasks
- Time Tracking
- Invoices
- Payments
- Expenses

---

## Entity Relationships

```text
LEADS
  │
  │ conversion
  ↓
CLIENTS
  │
  ├───────────────┐
  ↓               ↓
PROJECTS       INVOICES
  │               │
  ↓               ↓
TASKS          PAYMENTS
  │
  ↓
TIME TRACKING

CLIENTS
   │
   ↓
EXPENSES / FINANCIAL REPORTING
```
# Core Tables
## Leads

Stores prospective customers and their current sales/follow-up status.

## Clients

Stores centralized customer information.

## Projects

Connects clients to the work being delivered.

## Tasks

Stores individual project activities.

## Time Tracking

Records time spent on projects and billable work.

## Invoices

Tracks amounts billed to clients.

## Payments

Tracks collected revenue.

## Expenses

Tracks operational costs.

---

# Design Principles

The system was designed around:

- Centralized records
- Consistent identifiers
- Reduced duplicate information
- Clear entity relationships
- Structured tables
- Reusable calculations
- Reporting-ready data
A) App Name & Purpose
# CampusSpend – Student Finance Tracker

## Purpose
CampusSpend helps students track their daily expenses, visualize spending trends, and manage budgets effectively. 
It allows users to add, edit, delete transactions, search with regex, and see statistics for better financial awareness.
B) Contact Info
## Contact
- GitHub: https://github.com/tiffany-lina/FinanceTracker
- Email: tiffany@example.com
C) Data Model (JSON)
## Data Model
Each transaction record follows this structure:

{
  "id": "txn_0001",
  "description": "Lunch at cafeteria",
  "amount": 12.50,
  "category": "Food",
  "date": "2025-09-29",
  "createdAt": "2025-09-29T10:22:00Z",
  "updatedAt": "2025-09-29T10:22:00Z"
}

- `id` – Unique identifier
- `description` – Text describing the transaction
- `amount` – Numeric value
- `category` – One of: Food, Books, Transport, Entertainment, Fees, Other
- `date` – Transaction date (YYYY-MM-DD)
- `createdAt` / `updatedAt` – Timestamp of creation/update
D) Accessibility Plan
## Accessibility Plan
- Skip-to-content link for keyboard users
- Labels bound to all input fields
- Visible focus styles for keyboard navigation
- Status messages announced via `aria-live="polite"` or `assertive`
- Full keyboard navigation across all interactive elements
- Mobile-first layout for screen readers

--------------------------------------------------
|                  Header                        |
|               CampusSpend                      |
---------------------------------------------------
| Nav: Dashboard | Records | Add | Settings      |
---------------------------------------------------
|                  Dashboard                     |
|  Total Spent: $XXX     Top Category: Food      |
|  Last 7 Days Trend Chart                        |
---------------------------------------------------
|                  Search Bar                    |
|  [Regex Search Input Here]                     |
---------------------------------------------------
|                 Records List                   |
|  Card 1: Lunch at cafeteria | $12.50 | Food   |
|  Card 2: Chemistry textbook | $89.99 | Books  |
|  Card 3: Bus pass | $45.00 | Transport        |
|  ...                                           |
---------------------------------------------------
|                   Add Form                     |
|  Description: [__________]                     |
|  Amount:      [_____]                           |
|  Category:    [Dropdown]                        |
|  Date:        [YYYY-MM-DD]                      |
|  [ Add Transaction Button ]                     |
---------------------------------------------------
|                   Settings                     |
|  Budget Cap: [_____]                            |
|  Base Currency: [USD]                           |
|  Other Units: [Minutes/Pages]                  |
---------------------------------------------------
|                    Footer                       |
|                 © 2026 Tiffany                 |
---------------------------------------------------
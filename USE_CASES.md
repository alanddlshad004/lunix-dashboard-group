# Use Case Documentation — Lunix Smart Finance

## 1. System Overview
**System Name:** Lunix Smart Finance  
**Purpose:**  
Lunix Smart Finance allows users to manage personal and shared expenses, track settlements, view dashboards, and receive AI-generated financial insights such as automatic categorization and monthly summaries.

**Actors:**
- **User:** Creates, manages, and views expenses, both personal and shared.
- **Friends:** Participants added by the user to share and settle expenses.
- **AI Model:** Performs automatic categorization and generates financial summaries.

---

## 2. Actor Descriptions

| Actor | Description | Goals |
|-------|-------------|-------|
| User | Primary system participant who manages personal and shared finances. | Track expenses, share costs, view dashboards and reports. |
| Friends | Other registered users linked to shared expenses. | View shared expenses and settle outstanding payments. |
| AI Model | System intelligence used for categorization and report generation. | Automate organization and provide spending insights. |

---

## 3. Use Case Descriptions

| Use Case | Primary Actor | Description / Goal | Relationships |
|----------|---------------|-------------------|---------------|
| Login / Register | User | Allows users to create an account or authenticate. | Includes → Manage Profile |
| Manage Profile | User | Update personal details and account settings. | Included by → Login/Register |
| Add Friends | User | Add other users to enable shared expense tracking. | Extends → View Dashboard |
| Create Shared Expenses | User | Record shared expenses with selected friends. | Includes → Sync Data in Real Time; Extends → View Dashboard |
| View Shared Expenses | User / Friends | Displays all shared expenses and balances. | Extends → View Summary |
| Settle Payments | Friends | Confirm repayment for shared expenses. | Extends → View Shared Expenses |
| View Dashboard | User | Shows financial analytics, charts, and balances. | Includes → View Shared Expenses; Extends → View Summary |
| View Summary | User | Provides detailed financial analysis and breakdowns. | Extended by → Generate Summaries (AI) |
| Generate Summaries (AI) | AI Model | Creates monthly summaries and spending insights. | Extends → View Summary |
| Categorize Transactions (AI) | AI Model | Automatically categorizes expenses based on type. | Extends → Filter Transactions |
| Filter Transactions | User | Filter records by category, date, or amount. | Includes → Store Data Securely |
| Store Data Securely | System | Encrypts and safely stores all expense data. | Included by → Filter Transactions |
| Sync Data in Real Time | System | Updates shared expenses instantly across users. | Included by → Create Shared Expenses |

---

## 4. Relationship Rules
- **«include»** — the base use case always triggers the included use case.  
  **Example:** Login/Register → includes → Manage Profile

- **«extend»** — optional or additional behavior.  
  **Example:** View Dashboard → extends → View Summary

---

## 5. AI Model Involvement

| AI Function | Purpose |
|-------------|----------|
| Categorize Transactions | Automatically assigns expenses to categories such as food, transportation, or bills. |
| Generate Summaries | Produces monthly financial summaries and identifies spending patterns. |

---

## 6. Sample System Scenarios

### Scenario 1: Creating a Shared Expense
1. User logs into the system.  
2. User selects **Create Shared Expense**.  
3. System synchronizes data with all group members.  
4. User adds friends to the expense group.  
5. Expense is stored securely and appears in all users’ dashboards.

### Scenario 2: AI Summary Generation
1. User opens the dashboard.  
2. User selects **View Summary**.  
3. The AI model analyzes stored expenses and generates a financial report.  
4. The system presents categorized spending data and a monthly summary.

---
 the use case lucid link https://lucid.app/lucidchart/9cc262c0-c164-4bfa-bfd8-162377607a17/edit?viewport_loc=-1947%2C-2890%2C14664%2C6696%2C0_0&invitationId=inv_49600a68-53f2-4e11-946e-b6480374f028

 [/assets/firs.png] 

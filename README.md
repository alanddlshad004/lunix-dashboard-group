# Linux — Smart Expense Tracker

## Team Members
- **Ammar Arkan**  
- **Aland Dlshad**  
- **Zozan Ala**  
- **Rouliana Khalil**  

---

## Abstract
**Linux** is a smart web application that helps users record, manage, and analyze their incomes and expenses.  

It provides a real-time dashboard showing:
- Total balance  
- Monthly income and expenses  
- Interactive pie and bar charts  

Users can filter transactions by date or category, and export data to Excel or PDF.

The app also supports shared and group expenses:
- Add friends by username to split bills  
- Automatically calculate who owes what  
- Sync balances in real time  

An AI module automatically categorizes transactions and generates spending summaries to help users better understand their financial behavior.

---

## Goal
To make personal and shared financial management simple, automated, and transparent, eliminating the need for manual spreadsheets.

---

## Current Practice
Most people rely on notebooks, Excel sheets, or chat messages to track expenses.  
These methods are manual, error-prone, and don’t update automatically between users.

---

## Novelty
**Linux** combines:
- AI-powered automatic expense categorization  
- Real-time dashboards and summaries  
- Shared and group expense management  
- Exportable financial reports  

Its smart automation and collaboration features make it unique compared to regular budgeting apps.

---

## Effects
Linux promotes:
- Better financial awareness  
- Transparency in shared costs  
- Easier budgeting and saving  
- Clear visualization of money habits  

---

## Technical Approach

| Component | Technology |
|------------|-------------|
| Frontend | React.js |
| Backend | Node.js, Express.js |
| Charts | Chart.js |
| AI Module | Python Microservice |
| Database | MongoDB |

---

## Risks and Challenges
- Maintaining real-time synchronization between users  
- Ensuring AI accuracy in categorization  
- Handling large datasets efficiently  

---

## How to Run (for Developers)

```bash
# Clone the repository
git clone https://github.com/yourusername/linux-expense-tracker.git

# Go to the project folder
cd linux-expense-tracker

# Install dependencies
npm install

# Start the development server
npm start

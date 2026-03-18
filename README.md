# S-Processor School Management System (SP)

**S-Processor** is a school management and accounting system that simplifies fee tracking, generates student reports, and provides AI-powered remarks. It helps schools manage finances accurately, reduce errors, and automatically generate student reports. SP stands for **School Processor**.

Designed for school administrators, accountants, and teachers, S-Processor provides secure and structured data handling.

---

## Features

- Fee tracking and accounting
- Automatic balance calculation
- Student management system
- Financial reports and analytics
- AI-generated student remarks
- Secure and structured data handling

---

## Dashboard & Analytics

The system provides:

- Exam reports
- Accounting dashboard
- Collection sheets
- Student information
- Class management

### Main Dashboard

Quick access to core modules:

- **Exams Report** – View student academic performance
- **Accounting** – Manage school finances
- **Collection Sheets** – Track daily payments
- **Student Information** – Access student records
- **Class Information** – View class-level data
- **Houses** – Manage student grouping

Designed for simplicity — users can navigate without technical knowledge.

![Dashboard](dashboard_2.png)
![Accounting](accounting_dashboard.png)
![Reports](report.jpeg)

---

## What S-Processor Will Do

- Detect students who haven’t paid fees
- Show students with low payments
- Predict expected income
- Flag unusual payments (too low / too high)
- Show daily, weekly, monthly trends

---

## Tech Stack

- **Frontend:** React / HTML / CSS / JavaScript  
- **Backend:** Node.js / Express  
- **Database:** MongoDB / MySQL  
- **AI Integration:** OpenAI API or custom logic  
- **Other Tools:** Git, REST APIs

---

## Accounting & Fee Management

The accounting module helps eliminate errors in school fee tracking.

**Key Functions:**

- Record student payments
- Automatically calculate balances
- Generate receipts
- Track total income per student and class

### Fee Collection Report (Analytics View)

Includes:

- Date of payment
- Class (e.g., Basic 8, Basic 9)
- Student names
- Last payment made
- Total amount paid
- Remaining balance
- Receipt number

Example: Total income for Basic 8 — GHC 570.00

---

## Smart Fee Tracking Features

- ✅ Real-time balance calculation
- ✅ Prevents under/overpayment errors
- ✅ Daily payment tracking
- ✅ Class-based financial summaries
- ✅ Easy auditing and transparency

---

## Payment Navigation System

Guided flow for managing payments:

- **Pay Fees** – Record new payments
- **Show All Fees** – View all transactions
- **Show Fees Paid Today** – Daily tracking
- **Show Fees Per Class** – Class-level breakdown

**Workflow:**

1. Admin inputs student and financial data
2. System stores data in database
3. Accounting module calculates totals and balances
4. AI module analyzes student performance
5. System generates report cards with automated remarks

---

## AI & Analytics Functions

### 1. Detect Unpaid Students
```javascript
function getUnpaidStudents(students) {
  return students.filter(student => student.amountPaid === 0);
}

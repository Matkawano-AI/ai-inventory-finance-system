# AI-Assisted Inventory & Finance System

This project documents how **structured AI prompting and systems thinking**
were used to design, analyze, and improve an inventory and finance
tracking workflow for a small business.

The focus is on **decision support, automation logic, and reliability**—
not model training or ML experimentation.


## Problem Statement

The existing inventory and finance process relied heavily on:
- Manual data entry
- Multiple disconnected sheets
- Human memory for tracking stock movements
- Periodic, error-prone reconciliation

This resulted in:
- Inconsistent inventory counts
- Delayed financial visibility
- Higher risk of human error

## ✅ Solution (High-Level)

I designed an AI-assisted inventory and finance tracker that turns messy, manual logging into a structured, low-friction system.

- Centralized all product, stock, and transaction data into a single Google Sheet system.
- Used structured prompts with ChatGPT to design the schema, formulas, and edge-case rules (returns, damaged items, stock transfers).
- Added Google Apps Script automation (daily triggers and safety checks) so users can log sales, update stock, and generate summaries with minimal manual steps.
- Documented the system so non-technical users can operate it with clear instructions instead of needing to understand the formulas or code.

## How It Works (System Overview)

This project is an AI-assisted inventory and finance system designed for a real small business use case.  
It is built in Google Sheets, with Apps Script automations running in the background.

### Core workflow

1. **Data entry by non-technical users**
   - Team members only need to interact with simple input areas (dropdowns, protected ranges, and guided fields).
   - Common actions: adding new items, logging sales, updating stock movement, and recording expenses.

2. **Automated calculations & logic**
   - Stock levels are updated automatically when a sale or movement is logged.
   - Separate views for:
     - Current stock on hand  
     - Items in transit or reserved  
     - Historical transaction logs
   - Financial summaries (revenue, cost, profit) are calculated based on the latest data.

3. **Apps Script automations**
   - Time-based triggers (for example, daily) clean up or reset specific sheets safely.
   - Safety checks are built in to avoid accidental overwrites or data loss.
   - The system was iteratively tested using “mock days” to simulate real operations and patch hidden bugs.

4. **Dashboard / manager view**
   - A summarized view lets the owner quickly see:
     - Inventory health
     - Daily / weekly performance
     - Key red flags (e.g., low stock or missing entries)
   - This reduces manual checking and allows faster decisions.

### My role in the system design

- Translated a **messy real-world workflow** into a structured, automated system.
- Used **AI (ChatGPT) as a pair-designer**:
  - Broke down requirements into clear steps.
  - Designed the data model (tabs, columns, relationships).
  - Specified the behavior of each Apps Script function and trigger in detail.
- Iterated through multiple versions until the system became:
  - Stable in daily use  
  - Easy enough for non-technical users to operate  
  - Flexible enough to extend in future (e.g., more products, branches, or currencies).

  ## Tech Stack & Tools

- **Large Language Model:** ChatGPT (used as a design, analysis, and validation assistant)
- **Spreadsheet Platform:** Google Sheets / Excel
- **Automation:** Google Apps Script (time-based triggers, safety checks)
- **Methods:** Structured prompt engineering, workflow decomposition, rule-based logic
- **Documentation:** GitHub Markdown (clear instructions and design rationale)

## AI Prompt Engineering Highlights

AI was used as a **design and reasoning partner**, not as a replacement for business logic or automation.

My prompt engineering focused on:

- **Requirement decomposition**
  - Breaking vague business needs into concrete system rules
  - Clarifying assumptions (what counts as stock, when inventory changes, edge cases)

- **Command-based prompting**
  - Using role, task, and constraint structures to guide AI output
  - Forcing clarity on formulas, logic flow, and script behavior

- **Two-phase prompting (Plan → Execute)**
  - First prompting AI to analyze the problem and propose a plan
  - Only then generating formulas, rules, or script logic

- **Validation & self-check prompts**
  - Instructing AI to re-check outputs against constraints
  - Catching logical errors before implementation

These techniques allowed me to design a system that is **stable, explainable, and scalable**, rather than trial-and-error driven.

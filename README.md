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

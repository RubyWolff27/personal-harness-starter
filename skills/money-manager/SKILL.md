---
name: money-manager
description: My money manager for day-to-day finances. Use when I say "budget", "cash flow", "bills", "spending", "savings goal", "net worth" or "money check-in". Keeps a budget, a bills calendar, savings goals and a monthly net worth snapshot in one Google Sheet. General information only, not financial advice. Investing questions go to the investment-manager skill.
---

# Money manager

The household CFO: where the money goes, what's due, and whether the goals are on track. It keeps the numbers; I make the calls.

> **General information only, not financial advice.** This skill helps me organise and understand my own numbers. It doesn't know my full situation and isn't a licensed adviser. For advice on my circumstances, I'll see a licensed financial adviser (in South Africa, check the adviser is registered with the FSCA as an authorised financial services provider or representative).

## When to use
- Monthly money check-in (first weekend of the month).
- Setting or changing a budget or savings goal.
- "Can I afford ...?" and "where did my money go?"
- Before a big purchase, a pay rise, a move, or the end of the financial year.

## Where the numbers live
- **One Google Sheet:** `2 Areas/Money/Money tracker` in Google Drive. Start from `drive-templates/money-tracker.csv` in this kit (import it into Google Sheets: File > Import). Tabs: Budget, Bills, Goals, Net worth.
- Grok Bot, Claude (Google Sheets connector, beta) and ChatGPT (Google Drive app) can all read and update the Sheet. **Read first, propose changes, then update only after I say yes.**
- Totals only. **No account numbers, card numbers, logins or full statements in chat.** Round to the nearest rand.
- (ChatGPT path) ChatGPT's own **Finances** feature (connects bank accounts through Plaid) is **US only** as of 12 October 2026. Don't rely on it outside the US.

## Steps (monthly check-in)
1. **Brief.** Confirm the month and what I want out of it (for example "on track for the house deposit?").
2. **Read the sheet.** Last month's budget versus actual by category, bills paid and coming, goal balances, net worth.
3. **Cash flow.** Money in, money out, surplus or gap. Flag any category more than 10% over.
4. **Bills.** List the next 30 days of bills with due dates. Flag renewals worth shopping around (insurance, energy, phone).
5. **Goals.** For each goal: target, balance, monthly amount needed, on track or not.
6. **Net worth.** Add this month's snapshot row (assets minus debts). Show the trend over the last 6 to 12 months.
7. **Three actions.** No more than three, each small and specific. Mark which ones need a professional.
8. **Propose the sheet update** as a table. Update only after I approve.
9. **Memory.** Any decision (for example "cut takeaway budget to $300") goes to `decisions-log.md`.

## South African context (default; checked 12 October 2026)
- **Tax year** runs 1 March to the end of February. Filing season is through **SARS eFiling** or the SARS MobiApp. Keep IRP5, IT3(b) and retirement and medical certificates.
- **Retirement savings:** contributions to pension, provident and **retirement annuity (RA)** funds are deductible up to 27.5% of the greater of remuneration or taxable income, capped at **R430,000 a year** from 1 March 2026 (was R350,000). Excess carries forward.
- **Two-pot system** (since 1 September 2024): new contributions split one-third into a savings pot, two-thirds into a retirement pot. One savings-pot withdrawal per tax year, minimum R2,000, taxed at my marginal rate. Explain the cost before I touch it; a withdrawal is not "free money".
- **Tax-free savings account (TFSA):** **R46,000 a year** from 1 March 2026 (was R36,000), **R500,000 lifetime**. Over-contributions are taxed at 40%. Track contributions across all providers in the sheet.
- **Emergency fund** first: 3 to 6 months of expenses in an accessible account.
- Amounts in rand (R). Use SARS's own calculators and tables; link, don't invent.
- If I move country, swap in local equivalents and say so.
## Never
- Never give personal financial, tax or credit advice, or recommend a specific product or provider.
- Never move money, pay a bill, open an account or sign up for anything.
- Never ask for or store passwords, account numbers, card numbers or SA ID numbers or SARS tax reference numbers.

## Done when
- [ ] Budget versus actual, bills, goals and net worth are each covered.
- [ ] No more than three actions, each specific.
- [ ] The sheet update was approved before it was made.
- [ ] The "general information only" line appears in the output.

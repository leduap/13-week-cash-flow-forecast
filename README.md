# The 13-Week Cash Flow Forecast: templates and workbook

Spreadsheet versions of the templates and the workbook from *The 13-Week Cash Flow Forecast: A Field Guide for Controllers, Treasurers and Finance Managers* by Ashok Paudel (Corporate Finance Field Guides).

## What is here

| Folder | File | What it is |
|---|---|---|
| `workbook/` | `13-week_cash_flow_forecast_blank.xlsx` | The workbook from Chapter 17, blank: enter your own inputs and calendar |
| `workbook/` | `13-week_cash_flow_forecast_Kestrine_Q1_2027_worked.xlsx` | The same workbook with Kestrine's quarter (Q1 2027) as the worked example |
| `templates/` | `13-week_templates_blank.xlsx` | The 20 templates of Appendix A, one sheet per template, with an index |
| `templates/` | `template_NN-N_*.csv` | The same templates as CSV files, one per printed table (22 files; Templates 8.1 and 15.1 each have a continued table) |

## The workbook

The workbook follows the map in Chapter 17 (Template 17.1). It has thirteen tabs:

| Tab | Holds | Typed or calculated |
|---|---|---|
| Pack | The eight integrity checks, then the headline figures for the weekly pack (Chapter 13) | Calculated |
| Inputs | Window dates, opening balances, facility terms, floors, rates, holiday lists, sales plan, receivables schedule, collection curve, shipments, paydays, one-off register, indirect-method lines | Typed (shaded cells) |
| Calendar | One row per calendar day: banking day, week, test day, holiday name | Calculated |
| Receipts | Opening receivables, wholesale billing by day and the collection curve, card settlements | Calculated |
| AP | Shipments, supplier runs, ocean freight, operating suppliers, rent and premiums | Calculated |
| Payroll and tax | Paydays, net pay, federal deposits, state withholding, sales tax | Calculated |
| Customs | Entries by month, duty, periodic monthly statement dates | Calculated |
| Debt | Daily revolver interest and commitment fee, monthly payment, term loan | Calculated |
| Forecast | The daily engine (one row per day) and the weekly view (13 columns) | Calculated |
| Actuals | Bank receipts by row and week, with the variance classification, and the bank closing balance on each test day | Typed or imported |
| Variance | Forecast against actual by row and week | Calculated |
| Covenant | Net debt, LTM EBITDA, leverage, interest cover, room against the covenant and the board ceiling | Calculated |
| Memo | Items that fall after week 13 | Calculated |

The daily engine applies the revolver rule of Section 17.2 on banking days: below the minimum cash, draw the shortfall up to the limit; above the repayment threshold, repay the excess while anything is drawn. The weekly view sums the daily engine for flows and reads each week's test day for balances. Beneath the test-day rows it shows the lowest daily liquidity in each week and, for weeks with actuals, closing cash less the bank balance. Nothing on the weekly view is typed.

### Integrity checks

The top of the Pack tab shows PASS or FAIL for the eight checks of Section 17.3:

1. Roll-forward: opening cash + receipts - payments + net draws = closing cash, every week.
2. Bank: the forecast starts from the bank balance.
3. Limit: the revolver never exceeds the limit; unused facility is never negative.
4. Minimum: closing cash on banking days is never below the minimum while unused facility remains.
5. Calendar: every payment falls on a banking day; every week has exactly one test day.
6. Totals: the weekly view's totals equal the daily engine's totals.
7. Bridge: operating cash flow by the direct method equals the indirect method (Chapter 2). In the workbook the indirect-method lines are entered on the Inputs tab from the P&L and the balance sheet, and the check passes within a tolerance set there ($0.15M in the worked copy).
8. No typed numbers on the weekly view, the Pack or the Covenant tab.

The blank copy shows ENTER INPUTS until the Inputs tab is filled in.

## How to use it

1. Start from the blank copy: `workbook/13-week_cash_flow_forecast_blank.xlsx`.
2. On **Inputs**, enter the window dates, your opening balances and facility terms, and your banking holidays and federal holidays for the coming year (the lists in the blank copy are for 2027; check them every year).
3. Enter the sales plan, the receivables schedule, the collection curve, shipments, paydays and the one-off register. Adapt the source tabs to your own business: the worked example has one wholesale curve, one card settlement lag and one supplier pattern.
4. Recalculate and check that **all eight integrity checks show PASS** at the top of the Pack tab before you use the forecast.
5. Each week, save a dated read-only copy, enter the week's actuals on **Actuals**, and roll the forecast forward (Chapter 9).

The workbook uses WORKDAY, MAXIFS, MINIFS, SUMIFS and ISFORMULA. It works in Microsoft Excel 2019 or later, Microsoft 365 and LibreOffice Calc; Google Sheets opens it as well.

To check your reading of the book, open the worked copy: its weekly view reproduces Kestrine's base forecast (Table 8.1), Table 17.2 (week 7, day by day) and the covenant figures of Chapter 12.

## The figures

Kestrine Inc., Kestrine Outdoor Co. and every other company in the worked example are fictional companies invented for teaching. Their people, numbers, customers, lenders and events are made up. The calendar is the real 2027 calendar, used hypothetically; rates and terms are illustrative.

## Education only, not advice

These files are for education only. They are not accounting, legal, tax, investment or other professional advice. Rules and standards change; rely on your own counsel, tax advisers and auditors.

## Use

You may copy these templates and the workbook for your own work and your own team's use. Please do not republish or sell them. The full terms are in the LICENSE file.

Copyright © 2026 Ashok Paudel. All rights reserved, except as stated above.

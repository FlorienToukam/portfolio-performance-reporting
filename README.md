# Portfolio reconciliation and performance reporting

A contribution recorded as income can make a portfolio look more successful than it is. I used a constructed $1 million portfolio to trace that error and three others through the reporting process, from holdings and cash reconciliation to the quarter’s return calculations.

This practice case uses sector-return inputs from a PGIM Forage exercise. Account records, fees, cash flows, prices and reconciliation exceptions are constructed assumptions. They are not actual client records or PGIM investment results.

## Start here

1. Read the [quarterly performance report](Quarterly_Performance_Report.pdf).
2. Open the [Excel reporting model](Portfolio_Performance_Model.xlsx).
3. Review the simulated CSV records alongside the workbook's reconciliation and performance calculations. `Methods` records the assumptions and references.

## Main findings

The quarter ends December 31, 2021. After correcting four seeded exceptions, the portfolio's ending value is $1,059,338.96.

| Quarterly measure | Result |
| --- | ---: |
| Net time-weighted return | 0.9153% |
| Net money-weighted return | 0.8969% |
| Money-weighted less time-weighted return | -1.84 basis points |
| Closing reconciliation residual | $0.00 |

The largest reporting issue was a $100,000 contribution classified as income. Correcting it reduced the initially reported return. The other corrections addressed a missing purchase, an omitted fee and a stale price. The useful result was an accurate, reconciled report; the corrections did not improve the underlying investment performance.

## Return calculations

Time-weighted performance links subperiod returns after removing external-flow effects. Money-weighted performance uses dated investor cash flows and closing NAV. Excel XIRR produces an annualized rate of 3.6061%, which the workbook converts to the same 92-day quarter before comparison with time-weighted performance.

The money-weighted result reflects the amount and timing of a $100,000 contribution and $50,000 withdrawal. Fees reduce NAV and are not counted twice. Internal purchases and sales are not external investor cash flows.

## Reporting checks

All 49 dated asset records reconcile to independently generated reference records. The seven closing sleeves, including cash, agree with the simulated statement. Return differences against rounded statement calculations are below 0.001 basis point. The report explains each correction and includes questions for a portfolio review.

## Scope

The data covers a short practice period. Prices between monthly observations use an assumed path. Cash earns no interest, and taxes, foreign exchange and transaction costs are not modeled. The reference hurdle is an assumption rather than an observed market-index return. No GIPS compliance is claimed.

The original third-party task documents and model answers are not included here. This repository contains the reporting extension, simulated records and written findings. Calculation background: [GIPS Calculation Methodology](https://www.gipsstandards.org/wp-content/uploads/2021/03/calculation_methodology_gs_2011.pdf) and [Microsoft XIRR documentation](https://support.microsoft.com/en-us/excel/functions/xirr-function).

Updated October 1, 2026.

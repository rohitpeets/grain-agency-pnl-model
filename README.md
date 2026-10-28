# Grain Commission Agency – 2023 Season Financial Model

I was assistant operations manager at a grain commission agency in Punjab for the 2023 season. The agency sits between farmers and the government in MSP procurement. This model rebuilds that season into a P&L, a monthly cash-flow view, and the farmer-advances book.

Numbers are modeled from season records and official prices, not audited. Anything that wasn't recorded is labeled as an assumption.

## How the business makes money

- **Commission:** 3.5% of MSP value, paid by the government. (2.5% is the commonly cited rate; shown as a sensitivity.)
- **Processing:** farmers pay ₹30–35 per quintal for drying, cleaning, packing and loading. Mostly goes to labor.
- **Advances:** cash lent to farmers between crops for labor, seed, fertilizer and fuel, in return for bringing the harvest to the agency. Big clients (~600 t) pay 0%, others 3% a year.
- Government arranges transport and pays ~45 days after the crop lands. Sites are owned.

## Season

400 t wheat (Apr–May) + 3,725 t paddy (Oct–Nov) = **4,125 t**, worth **₹89.8M ($1.09M)** at MSP.

## Results (base case)

| | ₹ | USD |
|---|---:|---:|
| Commission revenue | 3.14M | $38.1K |
| Processing revenue (labor = fee) | 1.34M | $16.2K |
| Interest on advances | 0.05M | $600 |
| Net revenue | 3.19M | $38.7K |
| Overhead (manager, asst. manager, site-manager commission) | 1.01M | $12.2K |
| **Operating profit (to owner)** | **2.18M** | **$26.4K** |
| Peak cash tied up (Oct-23) | 6.57M | $79.6K |

- Profitable but cash-heavy. Peak cash tied up is 2.1x the season's net revenue, mostly from the paddy harvest and the 45-day payment lag.
- The advances lose money as loans: $600 interest vs ~$2,590 the cash would earn at the RBI rate. They pay off by locking in crop. The model puts commission on that volume at ~7.3x the cost, assuming 50% of volume came from borrowers and wouldn't have come otherwise.
- Commission rate is the biggest swing. At 2.5%, commission drops to $27.2K.

## Public inputs

| Input | Value | Source |
|---|---|---|
| Wheat MSP 2023-24 | ₹2,125/qtl | [PIB](https://www.pib.gov.in/PressReleasePage.aspx?PRID=1868760) |
| Paddy MSP 2023-24 | ₹2,183/qtl | [PIB](https://www.pib.gov.in/PressReleseDetailm.aspx?PRID=1930443) |
| INR/USD 2023 avg | 82.60 | [RBI Handbook, Table 135](https://rbi.org.in/scripts/PublicationsView.aspx?id=23309) |
| Cost of capital | ~6.5% (RBI repo, time-weighted 6.47%) | [RBI](https://www.rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=55267) |

## Assumptions

Processing labor cost, the 0%/3% borrower split, 6-month loan length, 50% committed volume, and site-manager commission on all volume. The advances book is the ~$80K I reconciled; total lending was larger.

## Files

- `Grain_Agency_2023_Financial_Model.xlsx` – Inputs, Volume & Revenue, Income Statement, Cash Flow & Working Capital, Advances Book, Sensitivity, Charts. Every number on the other sheets comes from Inputs.
- `Summary.pdf` – 2-page summary.

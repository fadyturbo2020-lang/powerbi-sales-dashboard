# Egypt Retail Sales Dashboard (Power BI + Excel)

Sales analysis of 1,200 retail orders across Egypt during 2025. First project of a three-part series (sales, costs, procurement).

> The dataset is **synthetic sample data generated for learning purposes** — it does not represent a real company. This is stated openly so the project shows real skills without claiming fake business experience.

## Status
| Component | State |
|---|---|
| Sample dataset (1,200 rows) | Ready |
| Excel analysis workbook (live formulas, native charts) | Ready — numbers verified |
| DAX measures | Ready |
| Step-by-step build guide | Ready |
| Power BI dashboard (.pbix) | **Pending** — built next in Power BI Desktop from this repo's pieces |

## Repo contents
| Path | What it is |
|---|---|
| `egypt_retail_sales_2025.csv` | 1,200-row sample sales dataset |
| `sales_analysis.xlsx` | Working Excel analysis: data, KPI summary with live formulas, charts |
| `measures.dax` | Ready-to-use DAX measures with comments |
| `build-guide.md` | Step-by-step guide to build the dashboard in Power BI Desktop |

## How to rebuild it
1. Open Power BI Desktop (free).
2. Get Data → Text/CSV → `egypt_retail_sales_2025.csv`.
3. Follow `build-guide.md` to model the data and add the measures.
4. Arrange the visuals as described, then save the `.pbix` here.

## Next steps
- Add a second dataset (e.g. customer returns) and relate it
- Publish to Power BI Service and link the live report here

## Series roadmap
1. **Sales analysis** — this repo
2. **Cost analysis** — cost structure, trends, and variance (starter Excel workbook ready)
3. **Procurement & supplier spend** — spend by supplier, category concentration, on-time delivery (starter Excel workbook ready)

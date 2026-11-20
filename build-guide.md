# Build guide: Egypt Retail Sales Dashboard

## 1. Load and clean (Power Query)
1. Get Data → Text/CSV → pick `data/egypt_retail_sales_2025.csv`.
2. Check types: `OrderDate` = Date, `Quantity` = Whole number, `UnitPrice` / `Discount` / `NetSales` = Decimal.
3. Remove any blank rows. Close & Apply.

## 2. Model
1. Create a Date table: Modeling → New table →
   `Date = CALENDARAUTO()` then mark it as a Date table.
2. Relate `Date[Date]` → `Sales[OrderDate]` (one-to-many).
3. (Optional) make small dimension tables for City and Category with `DISTINCT`, and relate them.

## 3. Measures
Copy the measures from `measures.dax` into the Sales table (New measure, paste each one).

## 4. Suggested report pages
**Page 1 — Overview**
- Cards: Total Sales, Total Orders, Average Order Value, Discount %
- Line chart: Sales by month (`Date[Date]` hierarchy → month)
- Bar chart: Sales by Category
- Slicers: Channel, Customer Segment

**Page 2 — Geography & products**
- Filled map or bar chart: Sales by City
- Table: Product, Total Sales, Total Quantity, sorted by sales
- Column chart: Sales MoM % by month

## 5. Polish
- Consistent colors, a clear title, and number formatting (thousands separators, EGP or plain numbers).
- Save the file as `egypt-retail-sales.pbix` in this repo (or keep the pbix local and add screenshots to an `images/` folder — screenshots make the repo look great).

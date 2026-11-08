# 📱 Mobile Sales Dashboard — Power BI

I built this dashboard to practice turning raw sales data into something a manager could understand in about ten seconds. It covers mobile phone sales by brand, model, city, payment method, customer rating, day of the week and month, and every visual responds to the filters.

> This is a learning project built on a sample dataset. Customer names were removed from the data, and brand names belong to their respective owners.

![Dashboard preview](dashboard.png)

## What I wanted to find out

- How much was sold overall, and across how many transactions?
- Which brands and phone models bring in the most money?
- Which cities are the strongest markets?
- How does quantity sold change from month to month?
- Which days of the week sell best?
- How do customers prefer to pay, and how do they rate their purchases?

## What's on the dashboard

| Section | Visual | What it tells you |
|---|---|---|
| Top strip | KPI cards | Transactions, total sales, total quantity and average sale at a glance |
| Left side | Month list | Filters the whole dashboard by month |
| Filter row | Slicers | Filter by mobile model, payment method, brand and day name |
| Total Sales by City | Map | Where the money is coming from |
| Total Quantity by Month | Line chart | How sales volume rises and falls through the year |
| Total Sales by Mobile Model | Column chart | Which models sell best |
| Transactions by Payment Method | Pie chart | Share of each payment type |
| Total Sales by Day Name | Area chart | Which days of the week bring the most sales |
| Transactions by Customer Rating | Funnel | How many transactions got each rating from 1 to 5 |
| Brand table | Table | Total sales, quantity and transactions for each brand |

## What I noticed

- The dataset has **3,835 transactions** and about **769M in total sales**.
- Sales are spread fairly evenly across brands. **Apple is slightly ahead** (about 161.6M), followed closely by Samsung (about 160.0M) and OnePlus (about 153.7M).
- **UPI is the most used payment method** at about 26%, but all four payment types are between 23% and 26%.
- **Saturday is the strongest sales day** and Wednesday the weakest.
- **Quantity peaks in July** and is lowest in February.

## How the data is set up

One table, `Sales-Data`, with brand, mobile model, city, payment method, date, day name, units sold, price per unit, customer age and customer rating. I wrote DAX measures on top of it: **Transactions**, **Total Sales**, **Total Quantity** and **Average**. I also designed the layout, the KPI icons and the logo myself.

## Try it yourself

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only).
2. Download `dashboard_powerbi.pbix` from this repo.
3. Open it and click through the filters to see how the numbers change.

## What I learned

- Planning the layout first (filters on the left, KPIs on top, details below) saves a lot of rework.
- Small details matter: clear chart titles, consistent names and a clean, relevant logo make a dashboard feel professional.
- Checking my own visuals found real mistakes, like a funnel chart that added up ratings instead of counting transactions.
- Writing DAX measures is cleaner than dragging raw columns into visuals.

## What I'd do next

- Add a proper Calendar table and show month-over-month change on the KPI cards.
- Show days of the week in Monday-to-Sunday order.
- Add drill-through so you can click a city and see its details.

## Tools used

Power BI Desktop · DAX · Power Query

## About me

Hi, I'm **Farhana Ashraf Ganaie**, learning data analytics and building projects to practice. I'd love feedback.

Connect with me on [LinkedIn](https://www.linkedin.com/in/farhana-ashraf-ganaie-8b188529b).

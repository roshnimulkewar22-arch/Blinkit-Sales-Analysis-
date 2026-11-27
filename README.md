# blinkit sales analysis

A single-page, dependency-free dashboard that analyses item-level sales for a Blinkit-style quick-commerce business. It turns raw rows into KPIs, charts and written insights for management.

**Live demo:** https://roshnimulkewar22-arch.github.io/blinkit-sales-analysis/

**All data is synthetic and for learning only. It is not real Blinkit data.**

## Project structure
```
blinkit-sales-analysis/
├── index.html   # the dashboard (HTML, CSS and JavaScript in one file)
└── README.md    # project description
```

## Tech
Plain HTML, CSS and JavaScript. Charts are drawn with inline SVG, so there are no libraries to install.

## What it analyses
| Area | What you see |
|---|---|
| KPIs | Total sales, average sales per item, items sold, average rating, average item visibility |
| Item type | Sales and share for each of 16 item types |
| Fat content | Low Fat vs Regular share of sales (donut) |
| Outlet size | Small, Medium and High outlets (donut) |
| Location tier | Tier 1, 2 and 3 locations |
| Outlet type | Sales, average sales, items, rating and visibility per outlet type |
| Establishment year | Sales by the year an outlet opened |
| Insights | Auto-written findings that update with the filters |

## Definitions
- **Total sales** = sum of Sales for the filtered rows (in ₹).
- **Average sales per item** = total sales ÷ number of items.
- **Average rating** = mean of Rating (1 to 5).
- **Item visibility** = share of display area given to an item. The dashboard shows the average.

## Run it
Open `index.html` in a browser. No build step.

## Use your own data
Click **Load your CSV**. The header row must use these column names (order does not matter, capitalisation is ignored):

`Item Fat Content, Item Identifier, Item Type, Outlet Establishment Year, Outlet Identifier, Outlet Location Type, Outlet Size, Outlet Type, Item Visibility, Item Weight, Sales, Rating`

Required: Item Fat Content, Item Type, Outlet Establishment Year, Outlet Location Type, Outlet Size, Outlet Type, Sales, Rating. Values like `LF` and `reg` are cleaned to Low Fat and Regular automatically. Fields must not contain commas. Use **Download sample CSV** for a ready template.

## Student tasks
1. Which item type earns the most? Is it also the best rated?
2. Compare outlet types. Which one should Blinkit expand?
3. Does outlet size or location tier explain higher sales per item?
4. How do Low Fat and Regular items compare in sales and rating?
5. Recommend one change to improve sales and support it with a chart.

## Deploy on GitHub Pages
Settings → Pages → Deploy from branch → main / (root).
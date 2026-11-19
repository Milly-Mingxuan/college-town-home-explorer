# Where Can You Afford a Home?

## What this site is for

Campus Home Explorer helps prospective buyers and people interested in college-town housing compare historical sale prices using one purchase budget. Users can adjust their budget, filter by state, and sort cities by the share of transactions within budget, median sale price, or number of matching sales.

## Live site

https://milly-mingxuan.github.io/college-town-home-explorer/

## Data notes

- The original CSV contains 35,442 completed sales. The analysis keeps the 35,371 rows with prices from $10,000 to $5,000,000 inclusive, across 18 cities. The 71 excluded transactions have unusually low or high reported prices.
- Budget match = number of eligible city sales at or below the selected budget / all eligible sales in that city. The overall share is weighted by the number of eligible sales. Median prices use all eligible sales in the city, regardless of budget.
- No street-address deduplication is performed; different units and repeated sales can share addresses. The original dataset listing ID identifies each sale.
- No dates or days-on-market calculation is used, because missing listing and contract dates are not random.
- Property type, lot size, bathroom count, tax amount, and living-area fields are not used because of documented reliability or outlier issues.
- This is a historical comparison, not an active inventory search or a measure of borrowing eligibility. All prices exclude financing and other transaction costs.
- The five supplied data files remain unchanged.

## Tools we used

ChatGPT Work Mode coding agent, plain HTML, CSS, and JavaScript, GitHub, and GitHub Pages. The browser reads the original CSV and computes results dynamically. See [AGENT_LOG.md](AGENT_LOG.md) for the collaboration record.

## Citation

College-town home sales dataset, version 1.0 (2026). University of Illinois-Deloitte Foundation Center for Business Emerging Technologies. Data collected March 2026. See [data description sheet](docs/data_description_sheet.md).

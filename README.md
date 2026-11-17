---
license: cc-by-4.0
pretty_name: Weekly Engineering Hiring Data
tags:
- jobs
- hiring
- salaries
- recruiting
- startups
size_categories:
- n<1K
configs:
- config_name: companies
  data_files: data/companies-hiring.csv
- config_name: salaries
  data_files: data/salary-by-role-level.csv
- config_name: weekly_totals
  data_files: data/weekly-totals.csv
---

# Weekly engineering hiring data

Free weekly data on who is hiring software engineers: open roles, new roles in the last 7 days and published pay. It covers 377 tech companies and YC startups with open engineering roles. Built from public career pages (Greenhouse, Lever, Ashby, Workday and 9 other applicant tracking systems) by [Matrixx Hiring Signals](https://matrixx-hiring-signals.pages.dev/?utm_source=github&utm_medium=referral&utm_campaign=dataset). Updated every Monday.

## This week (2026-11-17)

| Metric | Value |
|---|---|
| Open engineering roles | 6,269 |
| New roles, last 7 days | 426 |
| Companies hiring this week | 111 |
| Roles open 30+ days | 3,007 |
| Roles open 90+ days | 1,161 |
| Median published pay | $226k |

### Startups opening the most engineering roles

| Startup | New roles | Open roles |
|---|---:|---:|
| [Zip](https://matrixx-hiring-signals.pages.dev/companies/zip/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 6 | 10 |
| [Athelas](https://matrixx-hiring-signals.pages.dev/companies/athelas/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 5 | 32 |
| [Overview](https://matrixx-hiring-signals.pages.dev/companies/overview/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 4 | 33 |
| [Encord](https://matrixx-hiring-signals.pages.dev/companies/encord/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 4 | 16 |
| [Legora](https://matrixx-hiring-signals.pages.dev/companies/legora/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 3 | 52 |
| [HappyRobot](https://matrixx-hiring-signals.pages.dev/companies/happyrobot/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 3 | 20 |
| [ARQ](https://matrixx-hiring-signals.pages.dev/companies/arq/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 3 | 12 |
| [Alpaca](https://matrixx-hiring-signals.pages.dev/companies/alpaca/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 2 | 32 |
| [voize](https://matrixx-hiring-signals.pages.dev/companies/voize/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 2 | 12 |
| [Adaptyv](https://matrixx-hiring-signals.pages.dev/companies/adaptyv/?utm_source=github&utm_medium=referral&utm_campaign=dataset) | 2 | 11 |

### Median pay by role family

| Role family | Median | Published ranges |
|---|---:|---:|
| Infra / platform / SRE | $215k | 745 |
| ML / AI | $250k | 681 |
| Backend | $216k | 267 |
| Security | $230k | 254 |
| Engineering management | $273k | 252 |
| Full-stack | $210k | 175 |
| Data | $223k | 174 |
| Mobile | $239k | 71 |
| Frontend | $216k | 58 |

## Files

| File | Contents |
|---|---|
| `data/weekly-totals.csv` | Headline totals, one row per week |
| `data/salary-by-role-level.csv` | 25th, 50th and 75th percentile pay by role family and seniority (cells with fewer than 3 ranges dropped) |
| `data/companies-hiring.csv` | Every company with open engineering roles: open roles, new this week, remote roles, median pay |

## Method

- Jobs are read from each company's own career page every day.
- Only software engineering roles are kept.
- "New" means posted in the last 7 days.
- Pay is the midpoint of the published range, converted to yearly USD.

Full method: https://matrixx-hiring-signals.pages.dev/methodology.html

## License and citation

CC BY 4.0. Credit "Matrixx Hiring Signals" with a link to https://matrixx-hiring-signals.pages.dev/data/.

Free tools on the same data:
- [Salary benchmark](https://matrixx-hiring-signals.pages.dev/tools/salary-benchmark/?utm_source=github&utm_medium=referral&utm_campaign=dataset)
- [Startups hiring engineers this week](https://matrixx-hiring-signals.pages.dev/startups-hiring-engineers-this-week/?utm_source=github&utm_medium=referral&utm_campaign=dataset)
- [Weekly insights](https://matrixx-hiring-signals.pages.dev/insights/?utm_source=github&utm_medium=referral&utm_campaign=dataset)

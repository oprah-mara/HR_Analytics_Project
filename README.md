# HR Analytics Dashboard (Power BI)

An end-to-end HR analytics project that examines workforce makeup, employee attrition, performance and attendance for 120 employees across six departments and three locations (Lagos, Abuja, Port Harcourt).

![Dashboard overview](workforce%20overview%20dashboard.png)
![Dashboard overview](attendance%20dahsboard.png)
![Dashboard overview](performance%20dashboard.png)

## Business Questions

- Where is attrition highest, and why do employees leave?
- How do pay, performance and engagement relate to retention?
- Does attendance help predict who leaves?

## Key Findings

- **Attrition is 20.8%** (25 of 120 employees), concentrated in **Customer Service (54.5%)** and **HR (28.6%)**.
- **Lower pay means higher attrition:** employees earning ₦400k or less left at 34.6%, compared with 12.9% above ₦600k.
- **"Better Opportunity" is the top exit reason** (40% of exits), followed by Poor Management.
- **Performance and engagement were flat** from 2024 to 2025 (average rating 3.24/5, engagement about 75/100).
- **Attendance is uniform** (about 5.7% absence) across departments, locations and leavers, so it is not a useful early-warning signal here.

## Recommendations

1. Review pay bands and career paths in Customer Service.
2. Investigate HR Officer turnover (half of the role has left).
3. Audit management quality using exit data.
4. Track engagement and overtime as retention indicators.
5. Add validation to HR data entry to fix inconsistent categories and missing reviews.

## Dataset

`data/HR_PowerBI_Dataset.xlsx` contains three linked tables (joined on `EmployeeID`):

| Sheet | Rows | Description |
|---|---|---|
| Employees | 120 | Demographics, department, job title, salary, hire and exit dates, exit reason |
| Performance | 172 | 2024 and 2025 ratings, training hours, overtime hours, engagement score |
| Attendance | 1,975 | Monthly working days, absences, leave and late arrivals (Jan 2025 to Sep 2026) |

**Data cleaning:** standardised inconsistent text in Gender, Department and Location, and handled one missing salary.

## Tools

Power BI · Excel · DAX · Power Query

## How to Use

1. Download `dashboard/HR_Dashboard.pbix`.
2. Open it in Power BI Desktop.
3. If prompted, point the data source to `data/HR_PowerBI_Dataset.xlsx`.

## Full Report

See [`reports/HR_Analytics_Report.pdf`](reports/HR_Analytics_Report.pdf) for the complete analysis and limitations.

## Author

**Amarachi** · [GitHub](https://github.com/oprah-mara)

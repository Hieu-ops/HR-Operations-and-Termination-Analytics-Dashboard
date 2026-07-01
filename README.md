# HR Operations and Termination Analytics Dashboard

## Project Overview

This Power BI portfolio project analyzes **2,586 HR event records** to provide a clear view of workforce activity across companies, locations, event types, and time periods.

The project was designed to answer two practical HR questions:

1. What types of HR events occur most frequently, and how do they change over time?
2. What patterns can be identified within employee termination events?

The final report contains two dashboard pages:

- **HR Operations Overview**
- **Termination & Internal Mobility Analysis**

## Dashboard Preview

### HR Operations Overview

![HR Operations Overview](HR%20Operations%20Overview.png)

This page provides an overview of major HR activities, including hiring, terminations, internal transfers, evaluations, event trends, work locations, and company-level activity.

### Termination & Internal Mobility Analysis

![Termination and Internal Mobility Analysis](Termination%20%26%20Internal%20Mobility%20Analysis.png)

This page focuses on termination volume, voluntary exits, termination reasons, monthly patterns, and the job families with the highest number of recorded departures.

## Key KPIs

| KPI | Value |
|---|---:|
| Total HR Events | 2,586 |
| Hiring Events | 281 |
| Terminations | 1,023 |
| Internal Transfers | 481 |
| Evaluations | 478 |
| Voluntary Exits | 908 |
| Voluntary Exit Share | 89% |

> Hiring Events combine new hires and rehires.

## Business Questions

The dashboards were developed to explore the following questions:

- Which HR event types occur most frequently?
- How does HR activity change across months?
- Which companies and work locations generate the most HR events?
- What are the main reasons for employee termination?
- What proportion of termination events are voluntary?
- Which job families show the highest concentration of termination events?

## Dataset

- **Format:** CSV
- **Rows:** 2,586
- **Columns:** 42
- **Main subject:** HR decisions and workforce events

Relevant fields include:

- Employee code
- Employee work start date
- HR event type
- HR event reason
- Event effective date
- Company
- Job level
- Job family
- Work location

The dataset records HR events rather than monthly employee headcount snapshots. Therefore, the analysis uses **event counts** and does not calculate turnover or retention rates.

## Data Preparation

The dataset was cleaned and transformed in Power Query before visualization.

Main preparation steps included:

- Renaming technical fields into business-friendly labels
- Converting date fields into the correct data type
- Separating event codes from event descriptions
- Separating company codes from company names
- Standardizing unknown work locations
- Creating month fields for time-based analysis
- Checking blank and inconsistent values
- Creating reusable measures for KPI monitoring

Personally identifiable employee information should be removed or anonymized before publishing the dataset publicly.

## Dashboard 1: HR Operations Overview

The first dashboard summarizes workforce activity through five KPI cards and four supporting visuals.

### Main Visuals

- Monthly HR event trend by event type
- HR events by type
- HR events by work location
- HR events by company and event type

### Key Observations

- Termination was the largest event category, with **1,023 recorded events**.
- Internal transfers and employee evaluations were the next most common categories.
- HR activity was concentrated in **Hanoi**.
- January showed the highest recorded HR event volume.
- The TE company code represented the largest share of recorded activity.

## Dashboard 2: Termination & Internal Mobility Analysis

The second dashboard investigates employee termination events in more detail.

### Main Visuals

- Terminations by reason
- Terminations by month
- Terminations by job family

### Key Observations

- **908 of 1,023 termination events were voluntary**, representing approximately **89%** of all terminations.
- Employee-initiated termination was the dominant termination reason.
- Termination activity peaked in January and declined substantially in later months.
- Several job families showed a noticeably higher concentration of termination events than others.

These findings describe the distribution of recorded events and should not be interpreted as turnover rates because the dataset does not contain reliable headcount denominators.

## Tools and Skills Demonstrated

- Power BI
- Power Query
- DAX
- Data cleaning and transformation
- KPI development
- Dashboard design
- Trend analysis
- HR data analysis
- Business insight communication

## View the Full Report

[Open the exported Power BI report](HR%20Workforce%20Analysis.pdf)

The PDF includes both dashboard pages and can be viewed without Power BI Desktop.

## Project Limitations

- The dataset records HR events rather than complete workforce snapshots.
- Turnover rate, retention rate, and net headcount change cannot be calculated reliably.
- Some work-location values were missing or marked as unknown.
- The high event volume in January may reflect operational activity, historical data entry, or data migration and should be validated before drawing a causal conclusion.
- The analysis is descriptive and does not establish why employees left.

## Future Improvements

- Add employee headcount data to calculate turnover and retention rates
- Include department and manager-level comparisons
- Add tenure analysis using validated employment dates
- Add report filters and drill-through pages
- Publish a fully anonymized interactive version through Power BI Service
- Improve the visual theme and mobile layout

## Portfolio Summary

This project demonstrates the ability to transform raw HR event data into a structured Power BI report, develop business-focused KPIs, identify workforce patterns, and communicate findings through clear visual storytelling.

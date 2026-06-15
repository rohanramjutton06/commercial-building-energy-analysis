## View the Report

If the PDF preview does not load on mobile, download the report file directly from the project files.

Report file: `Github_Project_Upload/Building_Energy_Analysis.pdf`


# Small Commercial Building Energy Load Analysis and Solar Feasibility Study

This project analyses a simulated 30-day electricity demand profile for a small commercial building and assesses the impact of a 30 kW rooftop solar PV scenario.

The project was completed using Microsoft Excel and focuses on energy load analysis, peak demand, estimated electricity cost, emissions, overnight base load, solar self-consumption, exported solar energy, grid import reduction and simple payback.

## Project Overview

The aim of this project was to develop an Excel-based dashboard that could be used to understand how a small commercial building consumes electricity and how rooftop solar PV could reduce grid electricity import.

The dashboard uses half-hourly simulated load data over a 30-day period. A simplified 30 kW rooftop solar generation profile was modelled and compared with the building demand.

## Key Results

| Metric | Result |
|---|---:|
| Total energy used before solar | 8130 kWh |
| Peak demand | 34.90 kW |
| Estimated bill before solar | $2731.20 |
| Estimated emissions | 5691 kg CO₂ |
| Overnight base load | 2.39 kW |
| Solar PV size modelled | 30 kW |
| Grid import after solar | 2549 kWh |
| Solar self-consumption ratio | 81.29% |
| Estimated monthly solar benefit | $1626.99 |
| Simple payback | 1.84 years |

## Tools Used

- Microsoft Excel
- Excel formulas including SUMIFS, MAXIFS, AVERAGEIFS and MINIFS
- Excel charts and dashboard formatting
- PDF project report

## Methodology

The project used 30 days of half-hourly demand data. Energy use was calculated using:

`Energy (kWh) = Demand (kW) × Time (h)`

Since each interval was 30 minutes:

`Energy (kWh) = Demand (kW) × 0.5`

A simplified solar PV profile was then modelled and compared with the building demand.

Key solar calculations included:

`Net grid demand = Building demand - Solar generation`

`Solar self-consumed = MIN(Building demand, Solar generation)`

`Exported solar = MAX(Solar generation - Building demand, 0)`

`Grid import = MAX(Building demand - Solar generation, 0)`

## Assumptions and Limitations

- The load data is simulated for a small commercial building.
- Electricity demand is recorded in 30-minute intervals.
- A 30 kW rooftop solar PV system is modelled using a simplified daytime generation curve.
- Tariff values, emissions factor and system cost are assumed.
- The analysis does not include detailed electrical design, inverter losses, shading, weather variation, panel orientation, protection design, grid connection approval or roof structural assessment.

## Project Files

- `Commercial_Building_Energy_Analysis.xlsx` — Excel workbook and dashboard
- `Small_Commercial_Building_Energy_Analysis_Report.pdf` — short project report
- `dashboard_screenshot.png` — dashboard preview image

## What I Learned

This project helped me better understand how electrical load data can be used to analyse building energy behaviour, identify demand patterns, estimate electricity costs and assess early-stage rooftop solar PV feasibility.

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository contains sales forecasting and business planning for DYODE, an eCommerce agency providing consulting, web development, and digital marketing services primarily for Shopify and BigCommerce merchants.

## Key Files

### client-data.csv
Master client database tracking all client engagements with the following structure:
- **Client identification:** Client Name, Service (Development/Marketing/Consulting)
- **Status tracking:** Start, Added, Lost, Active flags
- **Contract details:** Contract Expiration, Last Renewal Date, Term Length, Contract Status (Active Term/Month-To-Month/Lost)
- **Financial data:**
  - For retainers: Avg Monthly $ (monthly recurring revenue)
  - For projects: Project Total (total project value)
  - Dev Minimum Hours, Dev Rate (for development services)
- **Timeline:** Added Date, Lost Date

**Important conventions:**
- Active = X means currently active client
- Added = X means added in 2025
- Lost = X means lost/churned in 2025
- Empty Term Length OR Term Length = 0 means month-to-month contract
- Project Total is used for one-time projects; Avg Monthly $ is for recurring retainers

### 2026-sales-forecast.md
Comprehensive sales forecast and strategic plan including:
- Historical revenue analysis (2018-2025)
- 2025 year-end projections
- Client churn analysis by service type
- 2026 growth targets by quarter and month
- Service-specific strategies (Development, Marketing, Consulting)
- Lead generation timeline and expectations (Martal partnership)
- eCommerce agency buying seasonality
- Risk assessments for key clients

## Data Calculations

### MRR Calculations
- **Retainer clients:** Use "Avg Monthly $" directly
- **Project clients:** Calculate monthly average as: Project Total ÷ Term Length (in months)
- **Month-to-month clients:** Identified by empty or 0 Term Length - these have higher churn risk

### Churn Analysis
When analyzing churn:
- Count clients where Lost = X
- Calculate by service type (Development/Marketing/Consulting)
- Consider both retainer losses and project completions
- Industry benchmark: 15-20% annual churn (DYODE's 2025: 35-40%)

### Revenue Forecasting
Key adjustments to consider:
- **Glenmorangie:** Typically quarterly payments ($22,500/quarter), Q3 2025 was anomaly at $22,500/month
- **Wyze:** 140 hours/month at $120/hr = $16,800/month (Q3-Q4 2025), risk of reduction if they hire in-house
- **Project revenue:** Naturally ends on completion - factor into churn calculations
- **Seasonality:** Q1 slow, Q2 strong, Q3 moderate, Q4 mixed (see forecast doc for details)

## Strategic Context

### Business Priorities (2026)
1. **Shopify Plus Partner Status:** Must close 4-6 Shopify Plus projects in 2026 to maintain Premium/Platinum partner badge
2. **Churn reduction:** Target reduction from 35% to 20% through better retention processes
3. **Contract shift:** Move from 75% retainer/25% project to 85% retainer/15% project
4. **Lead generation:** Martal partnership (Nov 2025 - Jan 2026) with 18 guaranteed SQLs

### Revenue Model
- **Development:** 61% of MRR, primarily Shopify Plus and BigCommerce Enterprise
- **Marketing:** 29% of MRR, focus on Klaviyo email, paid social, SEO
- **Consulting:** 6% of MRR, strategic advisory and fractional CTO/CMO
- **Target client:** eCommerce brands $10M+ revenue, $7-15k/month engagements

## Working with Forecasts

When updating sales forecasts:
1. Always recalculate MRR from client-data.csv as source of truth
2. Account for project wind-downs (check Added Date + Term Length)
3. Consider month-to-month clients as higher risk (no contract protection)
4. Factor in realistic sales cycles (30-60 days) and seasonal buying patterns
5. Cross-reference with historical churn patterns when projecting losses
6. Martal SQLs delivered ≠ immediate closes; account for conversion lag

## Important Business Context

- Peak revenue was $4.86M in 2022
- Currently experiencing 34% decline from peak over 3 years
- Primary challenge: High churn (35-40%) driven by too many month-to-month contracts and project dependency
- 2026 goal: Reverse decline with 38-42% MRR growth to $360-370k

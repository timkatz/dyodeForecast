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

**Important data structure notes:**
- **Total rows:** 58 (including header)
- **Unique clients:** 53 distinct companies
- **Active clients:** 30 unique clients (where Active = X)
- **Multiple service lines:** Some clients engage DYODE for multiple services, creating multiple rows:
  - AG Jeans: Development + Marketing (2 rows)
  - Great Star Tools: 2 Development services + Marketing (3 rows)
  - MadEngine (Fithsun): Marketing + Consulting (2 rows)
  - Tipsy Elves: Development + Consulting (2 rows)

**Important conventions:**
- Active = X means currently active client (30 unique clients as of Nov 2025)
- Added = X means added in 2025
- Lost = X means lost/churned in 2025
- Empty Term Length OR Term Length = 0 means month-to-month contract
- Project Total is used for one-time projects; Avg Monthly $ is for recurring retainers

**When discussing clients:**
- "Clients" or "unique clients" = distinct companies (53 total, 30 active)
- "Service rows" or "engagements" = individual service lines (58 total rows)
- "Client services" = the specific service type provided (Development, Marketing, or Consulting)

### cross-sell-strategy-2026.md
Detailed cross-sell strategy and account manager incentive program including:
- Analysis of 24 viable cross-sell targets (after excluding past service history)
- Revenue opportunity: $51-69k MRR from 8-10 cross-sells
- Account manager 5% commission on contract term value (not full year)
- Commission aligns with typical 3-6 month contract terms
- Cross-sell playbook and conversation starters
- Priority target client list with revenue potential
- Implementation timeline and success metrics

### past-service-history.md
Documents clients who previously tried and stopped additional services:
- Helps avoid wasted cross-sell efforts on poor prospects
- Tracks reasons for discontinuation when known
- Examples: Wyze, Tori Richard (stopped marketing), Stikwood (paused dev retainer)

### martal-targeting-strategy.md
Comprehensive targeting and messaging strategy for Martal lead generation partnership:
- Ideal Client Profile (ICP): Shopify Plus, $10M+ revenue, specific verticals
- Messaging framework and email templates
- Pain point-driven outreach approach
- Qualification criteria for SQLs
- Competitor positioning
- Success metrics and monthly check-ins

### client-referral-review-program.md
Credit-based incentive program for client referrals and Clutch reviews:
- Clutch reviews: $500 service credit (target: 10-15 reviews in 2026)
- Client referrals: 5-10% of first contract value in credits (target: 5-8 conversions)
- Tiered referral structure based on deal size
- Credit mechanics, expiration, and policies
- Expected ROI: 10-15x on referrals, 10-20x on reviews
- Integration with 2026 client acquisition strategy

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

### program-rollout-strategy.md
Coordinated rollout plan for all 2026 growth programs:
- Timeline: Internal prep (Dec 2025) → Soft launch (Jan 2026) → Full launch (Feb 2026)
- Email templates for account managers and clients
- Training session agenda (Dec 11, 90 min)
- Conversation scripts for AMs
- Success metrics dashboard
- Integration of cross-sell, referral, and review programs

### executive-summary-cofounders.md
Strategic high-level document for co-founder decision-making:
- Full financial visibility (MRR, revenue, projections)
- Three financial scenarios (Conservative, Base Case, Aggressive)
- Decision points requiring co-founders' approval by Dec 2
- Risk analysis and mitigation strategies
- Investment recommendations ($107-130k for $4.2M target)
- ROI expectations and strategic trade-offs

### executive-summary-management.md
Operational document for executive management team (has full financial visibility):
- Role-specific responsibilities by team (Account Management, Sales, Marketing, Delivery)
- Training and support details
- Success metrics by role
- FAQ section addressing common concerns
- More operational/motivational tone than co-founder summary
- Assumes management has access to full revenue and MRR data

### executive-summary-account-managers.md
Tactical execution guide for account management team:
- Earnings-focused (commission/credit opportunity front and center)
- Step-by-step playbooks for cross-sells, referrals, and reviews
- Includes specific revenue examples for commission calculations
- 30-day action plan with training prep requirements
- Recognition and career growth opportunities
- Designed for individual contributor execution (not strategic oversight)
- **NOTE:** Written before org structure clarification; references "Account Managers" which should be interpreted as "client-facing roles" (PMs, Director of Digital Marketing, Marketing Manager)

### incentive-structure-analysis.md
Initial analysis of commission fairness across roles:
- Identified fairness concerns about who can earn commissions during salary freeze
- 5 options analyzed (AM-only, overrides, company bonuses, role-specific, profit sharing)
- Hybrid approach recommendations
- **STATUS:** Superseded by revised-incentive-structure-simple.md after org structure clarification

### revised-incentive-structure-simple.md
Simplified incentive structure based on actual DYODE org structure:
- Client-facing roles: PMs, Director of Digital Marketing, Marketing Manager, Director of Operations
- Non-client-facing roles: Director of Project Management, Director of Web Development
- Three options: Simplest ($21-37k budget), Inclusive ($36-57k), Middle ($25-43k)
- Recommendation: "Simplest" option with all client-facing roles earning same commission structure
- Google Sheet tracking approach (simple, low overhead)
- Special provision: Director of Operations earns 3% on new client sales (in addition to cross-sell/referral commissions)
- **STATUS:** APPROVED - Option A (Simple, client-facing roles only)

### raise-unlock-framework.md
Salary freeze and raise unlock criteria based on profit margin:
- **Target:** 12-15% profit margin for 2 consecutive quarters
- **Unlock timeline:** Q4 2026 (best case) or Q1 2027 (standard case)
- **Historical context:** Includes full profit margin history (2018-2025)
  - 2024: 8.3% margin (first goal of 10%, came close)
  - 2025: 0.3% margin (tariffs hit in April, ended at breakeven)
  - 2020-2024 baseline: 6-8% margins with proper accounting
- **Raise structure:** 3-5% merit-based, performance-differentiated
- **Key principle:** Commission earnings don't count against raise eligibility
- **Communication:** Transparent quarterly updates on profit margin progress
- **STATUS:** FINAL - Ready for team communication

### option-a-implementation-plan.md
Execution roadmap for approved incentive structure (Option A):
- Summary of who earns what ($21-37k budget)
- Document updates required (6 strategy docs need revisions)
- Communication plan for different audiences
- Google Sheet tracker specification
- Next steps checklist
- **STATUS:** Ready to execute

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

### Leadership Structure

**Co-Founders:**
- Tim Katz and George

**Team Structure:**

DYODE is a small team with the following structure:

**Development Side:**
- **Director of Web Development** - Oversees web development team
- **Director of Project Management** - Oversees project managers (does not directly manage client accounts)
- **Project Managers (PMs)** - Client-facing, manage day-to-day relationships with development clients

**Marketing Side:**
- **Director of Digital Marketing** - Client-facing, directly oversees marketing engagements
- **Marketing Manager** - Client-facing, supports director, works together on all marketing accounts
- Small team (2 people total), both hands-on with clients

**Operations & Sales:**
- **Director of Operations** - Oversees company day-to-day operations + de facto account executive for inbound sales leads (builds proposals, closes deals)

**Important Notes on Structure:**
- **No dedicated "Account Management" team** - Client relationships are managed by Project Managers (dev side) and Director of Digital Marketing + Marketing Manager (marketing side)
- **Project Managers ≠ Account Managers** - PMs manage development client relationships, not a separate account management function
- **Director of Operations wears two hats** - Internal ops + sales/business development for new clients
- **Small, lean team** - Keep processes simple; complex tracking systems won't work well

### Company Performance

**Historical Context:**
- **2018-2019:** 38% profit margins (did NOT include co-founder salaries - not comparable)
- **2020:** Accounting changed to include co-founder salaries (30% margin, first "true" baseline)
- **2020-2022:** Hired aggressively during pandemic at premium salaries (bidding war for dev talent)
- **2021-2022:** Peak revenue $4.86M, but margins dropped to 6-8% (team scaled for $5M+ business)
- **2023-2024:** Revenue declined to $4.0M
  - **April 2024:** Laid off 10 people
  - **October 2024:** Gave raises to remaining team (balancing morale)
  - **2024 year-end:** 8.3% profit margin (close to 10% goal)
- **2025: Turbulent year**
  - Set 15% margin goal (business seemed to be recovering)
  - **April 2025:** Tariffs hit, business slowed dramatically
  - **Early 2025:** Forecasted -$200k profit loss (crisis mode)
  - **Froze raises** when performance deteriorated
  - Laid off 2 developers
  - **Year-end:** Avoided $200k loss, ended at 0.3% profit margin (breakeven)
  - Operating loss of -$27k, saved by $34k other income

**What Team Has Been Through (2024-2025):**
- April 2024: Layoffs (10 people)
- Oct 2024: Raises (morale boost after layoffs)
- 2025: Raises frozen (tariffs/performance decline)
- 2025: More layoffs (2 developers)
- Incredibly turbulent period for small team

**Current State (Nov 2025):**
- MRR: $292,946
- Active clients: 30 unique clients
- Projected 2025 revenue: ~$3.4M
- Profit margin: 0.3% (breakeven crisis)
- In salary freeze (no raises until profit margin recovers)

**2026 Goals:**
- Revenue: $4.2M
- MRR: $360-370k (38-42% growth)
- Profit margin: 12-15% (unlock raises when achieved for 2 consecutive quarters)
- Reverse 3-year decline trend
- Reduce churn from 35-40% to 20-25%

### Current Business Constraints

**Hiring Freeze:**
- Currently in place across all roles
- No salary raises during freeze period
- Creating need for performance-based compensation alternatives

**Budget:**
- Tight budget constraints
- Need to keep growth program investments lean and ROI-focused
- Prefer simple, low-overhead solutions

**Team Size:**
- Small, lean team
- Cannot support complex processes or extensive administrative overhead
- Simple Google Sheets tracking preferred over complex CRM workflows

### Metrics Sharing Strategy

**What's historically been shared with entire team:**
- **Profit margin %** - Overall company profitability
- **% to MRR goal** - Progress toward MRR needed to hit profit margin goals based on average monthly expenses
- **NOT shared:** Annual revenue figures, specific MRR numbers, client-level financials

**What should be shared with executive management team (monthly management meetings):**
- Full revenue details (annual revenue, MRR, projections)
- Client churn analysis and at-risk clients
- Detailed financial scenarios and investment decisions
- Strategic priorities and resource allocation

**What should be shared with entire team (monthly town halls):**
- Company performance against profit margin targets
- % to MRR goal (progress toward targets)
- Client wins and losses (count, not dollars)
- Program launches and team recognition
- Growth initiatives and how they contribute

**Important:** When creating documents for "executive management team," assume they have full financial visibility. When creating documents for "entire team" or "account managers," focus on actionable metrics and % to goal rather than absolute revenue/MRR numbers, unless the program specifically requires it (e.g., commission calculations).

### Incentive Program Considerations (2026)

**Client-Facing Roles (Eligible for Commissions):**
- Project Managers (manage development client relationships)
- Director of Digital Marketing (manages marketing client relationships)
- Marketing Manager (works hands-on with marketing clients)
- Director of Operations (handles new client sales, proposals, closes)

**Non-Client-Facing Roles:**
- Director of Project Management (coaches PMs, doesn't directly manage accounts)
- Director of Web Development (manages dev team, occasional technical client interaction)

**Key Principles:**
- Keep incentive structures simple and fair
- Commission opportunities should align with client-facing responsibilities
- Tight budget: Need to balance fairness with cost control
- Use Google Sheets for tracking (not complex CRM workflows)
- When updating incentive program documents, replace generic "Account Manager" references with actual client-facing role titles

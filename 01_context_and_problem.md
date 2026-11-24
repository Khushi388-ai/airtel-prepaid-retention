# 01. Company Context and Problem Identification

> Independent learning project using public information only. Not affiliated with Airtel. Figures come from news coverage and broker research (see [SOURCES.md](SOURCES.md)); verify against company filings.

## Company context
Bharti Airtel is India's second-largest telecom operator. India mobile is its biggest segment: Rs 30,943 crore revenue in Q2 FY27, more than 51% of consolidated revenue, with about 377 million India mobile customers. Postpaid customers are about 31 million, so most of the base is prepaid.

## How prepaid works
Customers pay upfront for a plan (for example 28 days of calling and data) and recharge when it ends. There is no contract, so Airtel earns only while customers keep recharging, and leaving is easy.

## How Airtel earns more per customer
The key metric is **ARPU** (average revenue per user per month). India mobile ARPU rose from Rs 256 to Rs 271 year on year. Two levers: raise prices or retire cheap plans, and shift customers to higher-value plans and postpaid. Customer segmentation lets Airtel design plans for different groups, but it creates risk for price-sensitive segments.

## Timeline of the triggering event
| Date | Event |
|---|---|
| Aug 2025 | Airtel retired its Rs 249 pack, making Rs 299 the cheapest daily-data entry pack |
| 12 Aug 2026 | Airtel withdrew the Rs 299, Rs 579, Rs 619 and Rs 649 plans; Rs 299 users were moved to the Rs 349 pack, about 16% higher |
| Q2 FY27 (Jul to Sep 2026) | Reported monthly churn rose from 2.6% to 2.9%; net subscriber additions fell from about 3.3 million to 0.7 million |
| Nov 2026 | Airtel restored a Rs 299 plan with 1 GB a day (many users previously had 1.5 GB) |

Analysts (Citi, JM Financial) linked the churn increase to the plan rationalisation. This is an analyst view, not confirmed by Airtel. Handset affordability may also have played a part.

## Problem statement
Airtel withdrew its Rs 299 prepaid plan in August 2026 to raise ARPU. Price-sensitive customers left in larger numbers than expected, and Airtel reversed the decision after the effect appeared in quarterly results.

**BA problem:** there was no visible early warning on who a plan change would push out, and no fast way to detect and respond once customers started leaving.

## Business goal
Keep the ARPU gains from plan changes while limiting churn among price-sensitive prepaid customers.

## Success measures (targets to validate)
- Monthly churn within 0.2 percentage points of the pre-change baseline
- Weekly net additions tracked for affected segments
- Complaint counts by category after any plan change

## Scope
- **In scope:** prepaid plan changes, customer notification, churn monitoring, retention offers
- **Out of scope:** postpaid, broadband, network quality, Airtel Africa

## Caveats
- Sources disagree on exactly which plans were withdrawn (some list Rs 319 and Rs 799 as well). This project uses the plans named in the 12 August reports.
- Whether the Rs 349 pack had identical benefits to the old Rs 299 pack is not confirmed here.
- Whether the plan withdrawal caused the churn is a hypothesis.

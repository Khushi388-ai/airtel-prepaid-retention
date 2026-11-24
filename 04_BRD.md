# Business Requirements Document: Airtel Prepaid Customer Retention

**Version:** 1.0 draft | **Prepared by:** Khushi Singh | **Basis:** public information only

Independent learning project, not affiliated with Airtel. Figures come from news coverage of Airtel's Q2 FY27 results and broker research; verify against company filings. Systems, thresholds and timelines are assumptions.

## 1. Purpose and scope
Defines the business requirements for managing churn risk when Airtel changes prepaid plans.
- **In scope:** prepaid plan changes, customer notification, churn monitoring, retention offers.
- **Out of scope:** postpaid, broadband, network quality, Airtel Africa.

## 2. Current business problem
- On 12 August 2026 Airtel withdrew the Rs 299 plan and others, moving Rs 299 users to the Rs 349 pack, about 16% higher.
- Reported churn rose from 2.6% to 2.9% and net subscriber additions fell from 3.3 million to 0.7 million. Analysts linked this to the plan rationalisation (a hypothesis, not confirmed by Airtel).
- The Rs 299 plan was restored in November 2026 with 1 GB a day, against the 1.5 GB many users previously had.
- **Root cause (hypothesis):** plan decisions are judged mainly on ARPU, with no built-in check on which customers a change will push out, no visible customer notice, and no churn monitoring fast enough to act before quarterly results.

## 3. Business objectives and success measures
- Keep the ARPU gains from plan changes while limiting churn among price-sensitive customers.
- Measures (targets to validate): churn within 0.2 percentage points of the pre-change baseline, weekly net additions tracked, complaint counts by category.

## 4. Stakeholders
| Stakeholder | Interest |
|---|---|
| Prepaid customers | Affordable plans, no surprises |
| Retention / CRM team | Fewer exits, win-back offers |
| Pricing and product managers | ARPU growth without churn |
| Finance | Revenue and quarterly results |
| Customer care | Complaints after plan changes |
| Retail and recharge partners | Sales and customer questions |
| Network / IT team | Systems to flag at-risk customers |

## 5. Proposed solution
Add a controlled process around every prepaid plan change: estimate churn risk by segment before approval, notify affected customers in advance with alternatives, track churn weekly after launch, and use a pre-set trigger to review or reverse the change. Offer a lower-data, lower-priced option to low-usage customers.

## 6. Systems impacted (assumed)
| System | Impact |
|---|---|
| Pricing / plan catalogue | Approval step with churn-risk check |
| Billing and recharge platform | Alternative plan suggestions at recharge |
| CRM / customer database | Segment and at-risk customer flags |
| Notification system (SMS, app) | Advance notices to affected customers |
| Analytics / reporting | Weekly churn dashboard and trigger alerts |
| Website and app | Plan display and messaging |
| Customer care tools | Complaint tagging by category |

## 7. Assumptions and dependencies
**Assumptions**
- Customer-level recharge, usage and plan history exists and supports segment analysis.
- A churn baseline per segment can be calculated from past data.
- Customers can be reached by SMS or app notification.
- Alternative plans can be offered without a long approval cycle.

**Dependencies**
- Data availability and quality from CRM and billing systems.
- Agreement between pricing, finance and retention on the churn limit.
- Notification channel capacity and regulatory rules on customer communication.
- Customer care agents trained on the new plan messaging.

**Risks:** too many alerts can slow decisions; risk estimates can be wrong for new customer groups; competitor offers may change the picture mid-review.

## 8. Business requirements
| ID | Requirement | Priority | Gap closed |
|---|---|---|---|
| BR1 | Estimate churn risk by segment before any plan is withdrawn or repriced | High | No pre-change churn test |
| BR2 | Notify affected customers in advance with their options | High | No visible warning |
| BR3 | Track churn weekly for affected segments after a change | High | Slow detection |
| BR4 | Offer a suitable alternative plan to low-usage customers | Medium | No low-need plan |
| BR5 | Trigger a review or reversal when churn crosses a set limit | High | No reversal rule |

## 9. Functional requirements
| ID | Requirement | Traces to |
|---|---|---|
| FR1 | Show pricing managers a segment-wise churn-risk estimate before a plan change is approved | BR1 |
| FR2 | Send an SMS/app notification to affected customers a set number of days before withdrawal | BR2 |
| FR3 | Show a dashboard of weekly churn and net additions for affected segments | BR3 |
| FR4 | Flag customers whose recharge value or frequency drops after a change | BR3 |
| FR5 | Recommend an alternative plan on the recharge screen when a plan is unavailable | BR4 |
| FR6 | Alert retention and pricing teams when the churn trigger is crossed | BR5 |

## 10. Non-functional requirements
- Notifications are delivered within 24 hours of scheduling.
- The dashboard refreshes at least daily.
- Customer data stays within existing privacy rules.

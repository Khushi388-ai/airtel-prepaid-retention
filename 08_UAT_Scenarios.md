# UAT Scenarios: Airtel Prepaid Customer Retention

Thresholds (7 days, 0.2 points, 8 weeks) are illustrative and should be validated with stakeholders.

| ID | Requirement | Scenario | Steps | Expected result |
|---|---|---|---|---|
| UAT1 | BR1, FR1 | High churn risk blocks approval | Pricing manager submits a plan withdrawal whose estimated segment churn risk is above the limit | Approval is blocked until a written justification is added |
| UAT2 | BR2, FR2 | Advance notice is sent | Schedule a plan withdrawal for a future date | Affected customers receive an SMS/app notice at least 7 days before |
| UAT3 | BR2, BR4 | Notice offers alternatives | Open the notice received by an affected customer | At least 2 alternative plans are listed |
| UAT4 | BR4, FR5 | Plan details are clear | Open an alternative plan on the recharge screen | Price, data and validity are all shown |
| UAT5 | BR3, FR3 | Weekly churn dashboard | Open the dashboard one week after a change goes live | Churn and net additions are shown per affected segment |
| UAT6 | BR5, FR6 | Trigger alert | Simulate weekly churn above baseline plus 0.2 points | Retention and pricing teams receive an alert |
| UAT7 | BR4, FR5 | Low-usage customer sees a lower-data plan first | Log in as a low-usage customer whose plan is unavailable | A lower-data, lower-price plan is shown first |
| UAT8 | BR5, BRU6 | Reversal is logged | Reverse a plan change after an alert | Reason and supporting data are saved in the log |

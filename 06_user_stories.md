# 06. User Stories and Acceptance Criteria

## US1: Pricing manager (BR1, FR1)
As a pricing manager, I want to see churn risk by segment before approving a plan change, so that I do not push out price-sensitive customers.
- Given a proposed plan change, when I open the approval screen, then I see estimated churn risk per segment.
- Given estimated risk above the set limit, when I try to approve, then the system blocks approval until I add a written justification.

## US2: Prepaid customer (BR2, FR2)
As a prepaid customer, I want advance notice when my plan will be withdrawn, so that I can choose what to do.
- Given my plan is scheduled for withdrawal, then I receive an SMS or app notification at least 7 days before.
- Given I open the notice, then it lists at least 2 alternative plans with price and benefits.

## US3: Retention analyst (BR3, BR5, FR3, FR4, FR6)
As a retention analyst, I want a weekly churn view for customers affected by a change, so that I can act early.
- Given a live plan change, then the dashboard shows weekly churn and net additions for affected segments.
- Given weekly churn above the trigger, then I receive an alert.
- Given customers whose recharge value or frequency drops after the change, then they are flagged as at risk.

## US4: Low-usage customer (BR4, FR5)
As a low-usage customer, I want a smaller, cheaper option, so that I do not pay for data I do not need.
- Given my plan is unavailable, when I open the recharge screen, then a lower-data plan is shown first.
- Given a plan is shown, then price, data and validity are all displayed clearly.

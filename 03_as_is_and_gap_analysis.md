# 03. As-Is Process, Root Cause and Gap Analysis

Airtel's internal process is not public. Steps marked *(assumed)* or *(inferred)* are hypotheses to validate with stakeholders.

## As-Is process: how a prepaid plan change works today
1. Pricing and product team decides to remove or reprice a plan to raise ARPU *(assumed)*
2. Plan is withdrawn from the website and app (12 Aug 2026)
3. Affected customers find out when they try to recharge *(inferred from reports that the changes surfaced through tipsters)*
4. Some customers move to the costlier plan, some downgrade, some leave *(assumed)*
5. Impact appears in quarterly results (churn 2.6% to 2.9%)
6. Airtel reverses the decision (Rs 299 restored in November)

## Pain points
1. **No like-for-like plan.** Customers who wanted the same benefits had no equivalent plan at any price. *(Check the benefits of the old Rs 299 and the Rs 349 pack on Airtel's site before relying on this.)*
2. **No visible notice.** The plans disappeared from the website and app, and the change was first reported by tipsters.
3. **Low-data users paying for data they do not need.** Customers with low needs have little reason to move to a costlier pack. *(Check how the unchanged Rs 199 and Rs 219 plans differ, since they may have served this group.)*

## Why customers might leave (ranked hypotheses, not confirmed)
1. Price increase on the entry plan
2. Better-priced competitor offers (Jio and Vi continued to offer Rs 299 plans)
3. Low-usage customers who do not value the extra data
4. Reduced data allowance on the restored plan (1 GB versus 1.5 GB)
5. Poor communication, so the change felt like a surprise

## Root-cause chain (5 Whys, hypotheses)
- Why did customers leave? Their entry plan was removed and the replacement cost more.
- Why was it removed? Airtel wanted to raise ARPU.
- Why was the risk not caught earlier? No visible churn check tied to plan changes.
- Why did that matter? Results arrive quarterly, so damage showed up after the quarter.
- **Root cause:** plan decisions are judged on ARPU, with no built-in check on who they will push out.

## Gap analysis
| Area | As-Is (observed or assumed) | Should be | Gap | Closed by |
|---|---|---|---|---|
| Impact prediction | ARPU is the main goal | Churn risk estimated per segment before launch | No pre-change churn test | BR1 |
| Customer notice | Plans vanish from site and app | Advance message with options | No visible warning | BR2 |
| Plan design | Entry plan removed | Option for low-data users | No like-for-like or low-need plan | BR4 |
| Monitoring | Quarterly results | Weekly churn tracking after a change | Slow detection | BR3 |
| Reversal rule | Decision reversed after results | Pre-set churn trigger | No trigger rule | BR5 |

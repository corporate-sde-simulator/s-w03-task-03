# PR Review - Sales report aggregation pipeline (by Sneha Jain)

## Reviewer: Pooja Reddy
---

**Overall:** Good foundation but critical bugs need fixing before merge.

### `salesAggregator.py`

> **Bug #1:** Group-by region uses first-letter match instead of full name so North and Northeast merge
> This is the higher priority fix. Check the logic carefully and compare against the design doc.

### `reportBuilder.py`

> **Bug #2:** Running total accumulates across report pages instead of resetting per page
> This is more subtle but will cause issues in production. Make sure to add a test case for this.

---

**Sneha Jain**
> Acknowledged. I have documented the issues for whoever picks this up.

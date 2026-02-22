# FINSERV-4130: Build sales report aggregation pipeline

**Status:** In Progress · **Priority:** High
**Sprint:** Sprint 25 · **Story Points:** 5
**Reporter:** Rajesh Kumar (Analytics Lead) · **Assignee:** You (Intern)
**Labels:** `backend`, `python`, `reports`, `feature`
**Task Type:** Feature Ship

---

## Description

The sales aggregator can fetch raw transaction data, but has **no report building capability**. Implement the `ReportBuilder` that groups, aggregates, and formats the data. Working `SalesAggregator` exists in `salesAggregator.py`.

## Acceptance Criteria

- [ ] `build_report()` groups data by specified dimensions (date, product, region)
- [ ] Aggregations: sum, average, count, min, max per group
- [ ] Report formatted as structured dict with totals row
- [ ] Date range filtering supported
- [ ] All unit tests pass

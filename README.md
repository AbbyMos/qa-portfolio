# qa-portfolio
QA tester resume and project portfolio

# 🧪 Beginner QA Tester Portfolio

> A hands-on QA testing portfolio focused on practical manual testing and basic SQL validation.

---

## 📁 What's Inside

| File | Description |
|------|-------------|
| `sql-validation-plan.md` | SQL queries to validate customer and order data |
| `qa-test-case-template.txt` | Manual test case matrix |
| `qa-bug-report-template.txt` | Structured bug report |
| `blog-entry-manual-testing.md` | Beginner reflection on QA testing |
| `qa-screenshot-log.txt` | Screenshot checklist |

---

## 🔍 SQL Test Preview

```sql
-- Orders per Customer
SELECT c.customer_id, c.name, COUNT(o.order_id) AS total_orders
FROM customers c
LEFT JOIN orders o ON c.customer_id = o.customer_id
GROUP BY c.customer_id, c.name;

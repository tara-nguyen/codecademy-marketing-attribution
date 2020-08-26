```sql
WITH first_touch AS (
  SELECT 
      user_id, utm_campaign, 
      MIN(timestamp) as first_touch
  FROM page_visits
  GROUP BY 1
)
SELECT
  utm_campaign, COUNT(*) AS count_ft
FROM first_touch
GROUP BY 1
ORDER BY 2 DESC;

WITH last_touch AS (
  SELECT 
      user_id, utm_campaign, 
      MAX(timestamp) as last_touch
  FROM page_visits
  WHERE page_name = '4 - purchase'
  GROUP BY 1
)
SELECT
  utm_campaign, COUNT(*) AS count_lt
FROM last_touch
GROUP BY 1
ORDER BY 2 DESC;
```

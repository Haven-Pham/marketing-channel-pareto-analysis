# Data

Two tables from the *Maven Fuzzy Factory* e-commerce dataset (Maven Analytics), a public, fictional dataset for
analytics training. They cover an online stuffed-toy retailer from March 2012 to March 2015.

## `orders.csv` (32,313 rows, one per order)

| Column | Description |
|---|---|
| `order_id` | Order identifier |
| `created_at` | Order timestamp |
| `website_session_id` | Session in which the order was placed |
| `user_id` | Anonymous visitor identifier |
| `primary_product_id` | First product added to the order |
| `items_purchased` | Number of items in the order |
| `price_usd` | Order revenue (USD) |
| `cogs_usd` | Cost of goods sold (USD) |

## `website_sessions.csv.gz` (472,871 rows, one per session; gzip-compressed CSV)

| Column | Description |
|---|---|
| `website_session_id` | Session identifier |
| `created_at` | Session start timestamp |
| `user_id` | Anonymous visitor identifier |
| `is_repeat_session` | 1 if the visitor had a previous session |
| `utm_source`, `utm_campaign`, `utm_content` | Paid-traffic tags; empty for untagged traffic |
| `device_type` | `desktop` or `mobile` |
| `http_referer` | Referring site; empty for direct type-in traffic |

The files are unchanged from the source except for compression.

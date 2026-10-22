# Webhook delivery retry backoff

Implements exponential backoff for webhook retries (ref #412).

- Base delay 500 ms, factor 2, cap 30 s
- 5 attempts, then dead-letter to meridian_dlq
- New metrics: webhook_retry_total, webhook_dlx_total

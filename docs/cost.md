# Cost Analysis (₹)

Cost estimates for **Global Synthetic Monitoring** in **Indian Rupees (₹)**.

## Production Environment

| Service | Monthly Cost (₹) | Notes |
|---------|------------------|-------|
| **CloudWatch Synthetics** | ₹15,000–40,000 | Canary runs |
| **Lambda** | ₹5,000–12,000 | Custom probes |
| **S3** | ₹2,000–5,000 | Screenshots/HAR files |
| **SNS** | ₹1,000–3,000 | Alerting |
| **CloudWatch** | ₹5,000–10,000 | Metrics/dashboards |
| **Total** | **₹28,000–70,000** | ~$350–875/month |

## Per-Canary Costs

| Frequency | Cost per Canary/month (₹) |
|-----------|--------------------------|
| Every 1 min | ₹3,500 |
| Every 5 min | ₹700 |
| Every 15 min | ₹250 |

## Cost Optimization

- **Optimize frequency** – Critical endpoints more often
- **Reduce screenshot size** – Compress images
- **Selective locations** – Monitor from key regions only
- **Consolidate canaries** – Multi-step scripts

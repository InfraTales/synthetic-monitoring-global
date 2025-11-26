# Security Overview

Security posture of **Global Synthetic Monitoring**.

## Canary Security

- **VPC deployment**: Private endpoint testing
- **IAM roles**: Least privilege per canary
- **Secrets**: Stored in Secrets Manager
- **No PII**: Avoid capturing sensitive data

## Data Protection

- **Encrypted storage**: S3 SSE-KMS
- **Screenshot redaction**: Mask sensitive areas
- **HAR sanitization**: Remove auth headers
- **Retention policies**: Auto-delete old data

## Access Controls

- **IAM policies**: Canary management
- **Resource policies**: Cross-account access
- **Audit logging**: CloudTrail integration

## Compliance

- SOC 2 monitoring requirements
- Uptime SLA evidence
- Incident response data

> See `SECURITY.md` for detailed configurations.

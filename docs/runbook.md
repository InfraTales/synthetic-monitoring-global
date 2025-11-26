# Runbook

## Deployment

```bash
npm install && cdk deploy --context environment=prod
```

## Creating Canary

```javascript
// canary.js
const synthetics = require('Synthetics');
const log = require('SyntheticsLogger');

exports.handler = async () => {
  const page = await synthetics.getPage();
  await page.goto('https://example.com');
  await page.waitForSelector('#main');
  log.info('Page loaded successfully');
};
```

## Multi-Location Setup

1. Deploy canaries to multiple regions
2. Configure CloudWatch cross-region dashboards
3. Set up composite alarms
4. Configure SNS for alerting

## Monitoring

- Check canary success rates hourly
- Review latency trends daily
- Investigate failures immediately

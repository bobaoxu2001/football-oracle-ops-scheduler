# Football Oracle ops scheduler

Hosted GitHub Actions pinger for https://football-oracle-agent.vercel.app/api/ops/tick

- Cadence: every 5 minutes
- Auth: `Authorization: Bearer $CRON_SECRET`
- Recurrence: GitHub-managed schedule
- Overlap: Mongo 90s tick lease (HTTP 409 is success)

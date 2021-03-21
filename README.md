# CTFTime Discord Bot using GitHub Actions
This is a GitHub action that periodically notifies the Discord channel of the most recent CTFs listed in [CTFTime](https://ctftime.org/). By default, it fetches data once a day and notifies the channel **if there are any differences from the last notification**. If you want to change the settings such as the interval to retrieve data, please edit [the workflow file](.github/workflows/ctftime.yml).

## Setup
1. Fork this repo.
2. Go to **Setting > Secrets** of the repo.
3. Add new repository secret.
   - Name: `DISCORDWEBHOOKURL`
   - Value: `(Your Discord Webhook URL)`

## Appendix: How to get a Discord webhook URL
1. Go to the channel setting **Integrations**.
2. Click **Webhooks > Create Webhook**.
3. Click **Copy Webhook URL**.
Cabot Stashboard Plugin
=====

This plugin allows you to send alerts to Stashboard. It needs OAuth credentials

Installation
----
1. Add cabot_alert_stashboard to the CABOT_PLUGINS_ENABLED list in *\<environment\>*.env
1. Add `STASHBOARD_TOKEN=<YOUR_OAUTH_TOKEN>` to *\<environment\>*.env
1. Add `STASHBOARD_SECRET=<YOUR_OAUTH_SECRET>` to *\<environment\>*.env
1. Add `STASHBOARD_URI=<YOUR_STASHBOARD_DOMAIN>` to *\<environment\>*.env
1. Set status codes and whether to auto-create services:
```
    STASHBOARD_NORMAL=up
    STASHBOARD_WARNING=warning
    STASHBOARD_ERROR=down
    STASHBOARD_CRITICAL=down
    STASHBOARD_CREATE_SERVICES=True
```
1. Deploy with fabric (`fab deploy -H ubuntu@example.com`)
1. Enable the plugin on whatever services you like

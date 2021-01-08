Copy `web_monitoring.py` to `/usr/lib/zabbix/externalscripts`
Install requirement software: `apt install python3-selenium chromium chromium-common chromium-driver`
Change ownership: `chown zabbix:zabbix /usr/lib/zabbix/externalscripts/web_monitoring.py`
Create new zabbix item:
- Type: External check
- Key: web_monitoring.py[-a https://example.com/]
- Type of information: Numeric (float)
- Units: seconds


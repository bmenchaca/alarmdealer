---
layout: page
title: "AlarmDealer.com Alarm Control Panel"
description: "Instructions how to integrate AlarmDealer into Home Assistant."
date: 2017-05-31 08:59
sidebar: true
comments: false
sharing: true
footer: true
logo: alarmdealer.png
ha_release: 0.24
ha_category: Alarm
---

The `alarmdealer` platform enables the ability to control a SecureSmart control panel. [ipdatatel.com/securesmart](http://ipdatadel.com/securesmart/).

To enable this, add the following lines to your `configuration.yaml`:

```yaml
# Example configuration.yaml entry
alarm_control_panel:
  platform: alarmdealer
  username: YOUR_USERNAME
  password: YOUR_PASSWORD
```

Configuration variables:

- **username** (*Required*): Username for the AlarmDealer account.
- **password** (*Required*): Password for AlarmDealer account.
- **name** (*Optional*): The name of the alarm. Default is the AlarmDealer alarm id.
- **code** (*Optional*): Specifies a code to enable or disable the alarm in the frontend.

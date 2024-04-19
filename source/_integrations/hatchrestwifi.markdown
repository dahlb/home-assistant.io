---
title: Hatch Rest Wifi
description: Instructions on how to integrate Hatch Rest sound machines over wifi within Home Assistant.
ha_category:
  - Media player
ha_iot_class: Cloud Push
ha_release: 2024.6
ha_codeowners:
  - '@dahlb'
ha_domain: hatchrestwifi
ha_config_flow: true
ha_platforms:
  - media_player
---

The Hatch Rest Wifi integration lets you control your sound machine over the local network. The following device models are currently supported:

- Rest+ (1-st generation)
- Rest-Mini

The media player platform of this integration allows you to turn the unit on/off, select the sound mode.

## Prerequisites

To set up the integration, you will need to know a username with password for hatch mobile app.


{% include integrations/config_flow.md %}

{% configuration_basic %}
username:
  description: "Username used to login to hatch mobile app."
  required: true
  type: string
password:
  description: "Password used to login to hatch mobile app."
  required: true
  type: string
{% endconfiguration_basic %}

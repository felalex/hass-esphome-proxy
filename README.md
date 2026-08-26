<h1>
  <img src="icon.png" alt="ESPHome logo" height="48" align="left">
  ESPHome Proxy
</h1>

<br clear="left">

ESPHome Proxy exposes an external ESPHome Device Builder instance through Home
Assistant Ingress.

## Installation

[![Open your Home Assistant instance and add this app repository.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Ffelalex%2Fhass-esphome-proxy)

1. Use the button, or add `https://github.com/felalex/hass-esphome-proxy`
   to the Home Assistant app store manually.
2. Install **ESPHome Proxy**.
3. Set the `server` option to the host and port of your ESPHome dashboard.
4. Start the app.

## Configuration

```yaml
server: esphome.local:6052
```

The `server` option must include both the hostname or IP address and the port.

Examples:

```yaml
server: esphome.local:6052
server: 192.168.1.60:6052
```

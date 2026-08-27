# ESPHome Proxy Documentation

ESPHome Proxy provides a Home Assistant Ingress panel for an ESPHome Device
Builder instance that runs outside Home Assistant.

## Options

### `server`

The upstream ESPHome dashboard address in `host:port` format.

```yaml
server: esphome.local:6052
```

Use an IP address when name resolution from the Home Assistant app network is
not reliable:

```yaml
server: 192.168.1.60:6052
```

## Troubleshooting

If the panel opens but the page does not load, confirm that Home Assistant can
reach the upstream ESPHome dashboard at the configured `server` address.

If ESPHome is reachable directly but not through the panel, check the app logs
for NGINX startup errors.

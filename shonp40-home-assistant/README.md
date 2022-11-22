# Initial configuration

In order to be able to access Home Assistant, you'll need to add the following lines to your `configuration.yaml` file to allow access through Umbrel's reverse proxy:

```yaml
http:
  use_x_forwarded_for: true
  trusted_proxies:
    - 10.21.0.0/16
```

The official Umbrel repo changes your `configuration.yaml` file location and can sometimes overwrite it between updates/reboots, which is why you'll need to set it manually here

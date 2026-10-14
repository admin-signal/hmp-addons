# Changelog

## 0.5.4

- Fix Tailscale status using fixed Supervisor metadata reads with the default role.
- Add staff-only status/start/stop for the fixed Community Tailscale add-on.
- Require manual boot, disabled watchdog and an enabled verified Running switch before Start.
- No Supervisor management role; preserve existing monitoring/device authorization.
- Separate amd64 and ARM64 images with automatic architecture selection.
- Optional staff pairing with device-generated key and persistent identity.

## 0.5.3

- Add staff-only status/start/stop for the fixed Community Tailscale add-on.
- Require manual boot, disabled watchdog and an enabled verified Running switch before Start.
- Preserve Supervisor permissions and existing monitoring/device authorization.
- Separate amd64 and ARM64 images with automatic architecture selection.
- Optional staff pairing with device-generated key and persistent identity.

## 0.5.2

- Separate amd64 and ARM64 images with automatic architecture selection.
- Optional staff pairing with device-generated key and persistent identity.

## 0.5.0

- Optional staff pairing with device-generated key and persistent identity.

## 0.4.0

- Group discovered readings by their Home Assistant device.
- Add selected existing readings with reviewed names, rooms and visibility.
- Recoverable monitoring activation; device control remains disabled.

## 0.3.2

- Add Home Assistant telemetry subscription and capture diagnostics for durable mode.
- Log telemetry publication acknowledgment without exposing entity IDs or state values.

## 0.3.1

- Add native/durable MQTT connection and subscription diagnostics.
- Log initial status publication and sanitized native transport failures.

## 0.3.0

- Optional stored-event delivery and appliance health reporting.

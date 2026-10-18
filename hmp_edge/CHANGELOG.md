# Changelog

## 0.5.7

- Expand remote discovery from 100 to 1000 readings so later-sorted battery/RSSI entities are available.
- Retain the 120 KiB MQTT response budget and explicit partial-list reporting, with efficient payload fitting.
- Requires the expanded Cloud discovery validator before this add-on update.
- Preserve persistent data, explicit reading permissions, private administration and amd64/ARM64 selection.

## 0.5.6

- Identify enabled Z-Wave node RSSI diagnostics through Home Assistant registry metadata.
- Associate signal-strength readings with their physical devices for the HMP Admin battery/RSSI screen.
- Reuse explicitly authorized, change-suppressed telemetry with dBm units and startup/reconnect readings.
- Preserve persistent data, permissions, private administration and amd64/ARM64 selection.

## 0.5.5

- Remove a configured device and all its HMP readings while leaving it paired in Home Assistant.
- Resume interrupted removals and confirm completion after the running registry reloads.
- Reject old onboarding/removal requests after fresh onboarding.
- Preserve existing appliance identity, permissions, private administration and amd64/ARM64 selection.

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

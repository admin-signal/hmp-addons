# HMP Edge

Contact your Signal Home administrator for installation and provisioning. Never start two appliances with the same identity.

## Remove from HMP

Administrators can remove a configured device and all its HMP readings, then discover and onboard it again. Removal leaves the device paired in Home Assistant. Wait for HMP to confirm removal before discovering again; pending removal can be resumed from Sensor onboarding.

## Optional Tailscale access

HMP Admin staff can check, start and stop the existing Community Tailscale add-on. In HAOS, disable Tailscale Start on boot and Watchdog, and enable its Running switch under the Home Assistant Supervisor integration. HMP refuses Start until it verifies these settings. Starting from HMP does not enable automatic startup; a host reboot leaves Tailscale stopped.

## Sensor health

HMP Admin Sensor health shows last-reported battery and RSSI readings by physical device. Enable diagnostic entities in Home Assistant, then explicitly add each reading through HMP Sensors with monitoring enabled. Customer visibility can remain off. Battery devices may report infrequently; missing RSSI alone does not mean offline. Cloud support must be updated before this Edge release.

## Discovery capacity

Remote discovery supports up to 1000 readings while retaining a 120 KiB MQTT response budget. Oversized lists remain explicitly marked partial. Update Cloud first, then update this add-on and run Discover devices in HMP. Explicitly approve each reading before telemetry is enabled.

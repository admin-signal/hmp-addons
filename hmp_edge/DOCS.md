# HMP Edge

Contact your Signal Home administrator for installation and provisioning. Never start two appliances with the same identity.

## Optional Tailscale access

HMP Admin staff can check, start and stop the existing Community Tailscale add-on. In HAOS, disable Tailscale Start on boot and Watchdog, and enable its Running switch under the Home Assistant Supervisor integration. HMP refuses Start until it verifies these settings. Starting from HMP does not enable automatic startup; a host reboot leaves Tailscale stopped.

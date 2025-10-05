# GrowWire
ESPHome config for Growatt TL3-S inverters over RS-485/Modbus RTU (ESP32).
- Input Registers only (Function 4) with correct scaling
- L-N voltages (auto-converted from L-L if needed)
- Per-phase power + PAC, daily/total energy
- Inverter & IPM temperatures
- Fast updates with safe throttling
- Secrets via `secrets.yaml`
- HA dashboard + wiring/register docs included

## Quick start
1) Copy `esphome/secrets.example.yaml` → `esphome/secrets.yaml` and fill:
   - `wifi_ssid`, `wifi_password`, `api_key_base64`, `ota_password`
2) Put `esphome/growatt.yaml` into your ESPHome folder and compile/upload.

Docs in `docs/`.

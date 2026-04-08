# Fabian-compatible package set

This package entrypoint preserves the existing `deyeesp32` / `deye-...` Home Assistant entity naming style used by the local ESPHome configuration while still using the repository package layout.

## Include this file

```yaml
packages:
  deye_fabian: !include github://BurnSkat/esphome-deye-inverter/pv_inverter/deye_hybrid_3p_lv_fabian.yaml@main
```

## Expected local substitutions / base config

Use your local device YAML for:
- `esphome:`
- `esp32:`
- `logger:`
- `api:`
- `ota:`
- `wifi:`
- `uart:`
- `modbus:`
- `modbus_controller:`

The package entrypoint already defines:
- `name: deyeesp32`
- `friendly_name: DeyeESP32`
- `device_type: deye`
- `modbus_controller_id: sg1334p`

## Custom package paths

- `pv_inverter/deye_hybrid_3p_lv_fabian.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/battery.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/grid.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/load.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/work_mode.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/device.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/inverter.yaml`
- `pv_inverter/packages_fabian/deye_hybrid_3p/pv.yaml`

# 1.6" 480×480 AMOLED MIPI module (ST7802) — documentation & samples

**简体中文：** [`README.md`](README.md)

---

> This repository provides **sample projects** for this module, together with datasheets, specifications, and interface / bring-up documentation for selection reference and integration.

## Product overview

| Item | Description |
|:--|:--|
| Module | 1.6-inch **AMOLED** panel, **480×480** resolution |
| Interface | **MIPI** |
| Driver IC | **ST7802** |
| Spec ID | **`1.6-amoled-480x480-mipi-st7802`** is the common product designation in documentation |

---

## Repository layout

### Top-level

| Path | Contents |
|:--|:--|
| `docs/` | Datasheets, specifications, interface and initialization documentation |
| `examples/` | **Sample projects** grouped by feature |

### `examples/` layout

| Location | Description (internal package folder) |
|:--|:--|
| `examples/` root | **ESP-IDF代码** (esp-lvgl-port + LVGL9) |
| `with-te/` | Tear-related samples (**屏幕防撕裂代码**) |
| `eaf/` | EAF animation (**EAF动画代码**) |
| `display-touch-test/` | Display and touch bring-up tests (**显示和触摸单独测试程序**) |

### Sample project paths

#### Baseline (`examples/` root)

| Description | Path |
|:--|:--|
| esp-lvgl-port + LVGL9 | `examples/esp32p4-idf5_st7802-mipi_esp-lvgl-port_lvgl9/` |

#### Tear-related (`with-te/`)

| Description | Path |
|:--|:--|
| LVGL9 common demo | `examples/with-te/esp32p4-idf5_st7802-mipi_lvgl9-common-demo/` |

#### EAF (`eaf/`)

| Description | Path |
|:--|:--|
| esp-lv-eaf-player | `examples/eaf/esp32p4-idf5_st7802-mipi_lvgl9_esp-lv-eaf-player/` |

#### Display and touch tests (`display-touch-test/`)

| Description | Path |
|:--|:--|
| ST7802 MIPI display test | `examples/display-touch-test/esp32p4-idf5_st7802-mipi-dsi/` |
| CST9220 touch I2C test | `examples/display-touch-test/esp32p4-idf5_cst9220-i2c/` |

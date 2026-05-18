# 1.6 寸 480×480 AMOLED MIPI 模组（ST7802）资料与示例

**English：** [`README_EN.md`](README_EN.md)

---

> 本仓库提供该模组的 **示例工程**，以及数据手册、规格与接口说明等资料，便于选型参考与集成开发。

## 产品概要

| 项目 | 说明 |
|:--|:--|
| 模组规格 | 1.6 英寸 **AMOLED**，分辨率 **480×480** |
| 接口 | **MIPI** |
| 驱动芯片 | **ST7802** |
| 规格标识 | 产品资料中常用 **`1.6-amoled-480x480-mipi-st7802`** 表示本规格 |

---

## 仓库结构

### 顶层目录

| 路径 | 说明 |
|:--|:--|
| `docs/` | 数据手册、规格说明、接口与初始化相关文档 |
| `examples/` | 按功能分类的 **示例工程** |

### `examples/` 分类

| 分类 | 说明（对应内部资料目录） |
|:--|:--|
| `examples/` 根目录 | **ESP-IDF代码**（esp-lvgl-port + LVGL9） |
| `with-te/` | **屏幕防撕裂代码** |
| `eaf/` | **EAF动画代码** |
| `display-touch-test/` | **显示和触摸单独测试程序** |

### 示例工程路径

#### 基础（`examples/` 根目录）

| 说明 | 路径 |
|:--|:--|
| esp-lvgl-port + LVGL9 | `examples/esp32p4-idf5_st7802-mipi_esp-lvgl-port_lvgl9/` |

#### 屏幕防撕裂代码（`with-te/`）

| 说明 | 路径 |
|:--|:--|
| LVGL9 通用演示 | `examples/with-te/esp32p4-idf5_st7802-mipi_lvgl9-common-demo/` |

#### EAF动画代码（`eaf/`）

| 说明 | 路径 |
|:--|:--|
| esp-lv-eaf-player | `examples/eaf/esp32p4-idf5_st7802-mipi_lvgl9_esp-lv-eaf-player/` |

#### 显示和触摸单独测试程序（`display-touch-test/`）

| 说明 | 路径 |
|:--|:--|
| ST7802 MIPI 显示测试 | `examples/display-touch-test/esp32p4-idf5_st7802-mipi-dsi/` |
| CST9220 触摸 I2C 测试 | `examples/display-touch-test/esp32p4-idf5_cst9220-i2c/` |

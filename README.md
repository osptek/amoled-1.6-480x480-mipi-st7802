<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK 1.6″ AMOLED 480×480（ST7802 · MIPI）</h1>

<p align="center"><b>圆形 AMOLED 模组 · MIPI DSI · ST7802</b></p>

<p align="center"><a href="./README_EN.md">English</a> | 简体中文</p>

<p align="center">
  <img alt="Size: 1.6 inch" src="https://img.shields.io/badge/Size-1.6%22-3498DB?style=flat-square" />
  <img alt="Resolution: 480x480" src="https://img.shields.io/badge/Resolution-480%C3%97480-8E44AD?style=flat-square" />
  <img alt="Interface: MIPI" src="https://img.shields.io/badge/Interface-MIPI-27AE60?style=flat-square" />
  <img alt="Driver: ST7802" src="https://img.shields.io/badge/Driver-ST7802-E7352C?style=flat-square" />
</p>

<p align="center"><img alt="OSPTEK 1.6 寸 480×480 AMOLED MIPI 模组（ST7802）宣传图" src="./images/product.png" width="640" /></p>

## 目录

- [产品简介](#产品简介)
- [规格参数](#规格参数)
- [示例工程](#示例工程)
- [仓库结构](#仓库结构)
- [相关资料](#相关资料)
- [购买链接](#购买链接)
- [技术支持](#技术支持)

---

## 产品简介

OSPTEK **1.6 寸 480×480 AMOLED** 是一款 **MIPI DSI** 接口彩色显示模组，显示驱动为 **ST7802**，触摸驱动为 **CST9220**。方形分辨率适合圆形穿戴表盘与紧凑 HMI 等场景。

规格标识（仓库名）：`1.6-amoled-480x480-mipi-st7802`

当前模组版本：**AM160Q480480LK4**。电气与外形细节以 [`docs/AM160Q480480LK4.pdf`](./docs/AM160Q480480LK4.pdf) 为准。

## 规格参数

| 项目 | 规格 |
| ---- | ---- |
| 尺寸 | 1.6 英寸 |
| 类型 | AMOLED（彩色） |
| 分辨率 | 480×480 |
| 接口 | MIPI DSI |
| 驱动 IC | ST7802 |
| 触摸驱动 | CST9220 |

> 完整外形尺寸、FPC 定义、供电与时序以产品规格书 / 驱动手册为准。

## 示例工程

| 说明 | 路径 |
| ---- | ---- |
| ESP32-P4 · ST7802 MIPI + esp-lvgl-port / LVGL9 | [`examples/esp32p4-idf5_st7802-mipi_esp-lvgl-port_lvgl9/`](./examples/esp32p4-idf5_st7802-mipi_esp-lvgl-port_lvgl9/) |
| ESP32-P4 · LVGL9 防撕裂演示 | [`examples/with-te/esp32p4-idf5_st7802-mipi_lvgl9-common-demo/`](./examples/with-te/esp32p4-idf5_st7802-mipi_lvgl9-common-demo/) |
| ESP32-P4 · EAF 动画播放 | [`examples/eaf/esp32p4-idf5_st7802-mipi_lvgl9_esp-lv-eaf-player/`](./examples/eaf/esp32p4-idf5_st7802-mipi_lvgl9_esp-lv-eaf-player/) |
| ESP32-P4 · ST7802 MIPI 显示测试 | [`examples/display-touch-test/esp32p4-idf5_st7802-mipi-dsi/`](./examples/display-touch-test/esp32p4-idf5_st7802-mipi-dsi/) |
| ESP32-P4 · CST9220 触摸 I2C 测试 | [`examples/display-touch-test/esp32p4-idf5_cst9220-i2c/`](./examples/display-touch-test/esp32p4-idf5_cst9220-i2c/) |

## 仓库结构

```text
1.6-amoled-480x480-mipi-st7802/
├── README.md
├── README_EN.md
├── MODULE_VERSION.md
├── LICENSE
├── images/          # README 用图
├── docs/            # 规格书、驱动手册、初始化等
└── examples/        # 示例工程
```

## 相关资料

### 本产品资料

| 资料 | 链接 |
| ---- | ---- |
| 产品规格书（AM160Q480480LK4） | [`docs/AM160Q480480LK4.pdf`](./docs/AM160Q480480LK4.pdf) |
| 驱动 IC 数据手册（ST7802） | [`docs/ST7802_DataSheet_V0.3.pdf`](./docs/ST7802_DataSheet_V0.3.pdf) |
| 触摸 IC 数据手册（CST9220） | [`docs/CST9220_Datasheet_V1.0.pdf`](./docs/CST9220_Datasheet_V1.0.pdf) |
| 初始化序列（文本） | [`docs/Truly160_480x480_ST7802N_AMOLED_Mipi_init.txt`](./docs/Truly160_480x480_ST7802N_AMOLED_Mipi_init.txt) |
| 时序参数参考图 | [`docs/Panel_Parameter_timing.png`](./docs/Panel_Parameter_timing.png) |
| 转接板原理图截图 | [`docs/adapter-board-schematic.png`](./docs/adapter-board-schematic.png) |
| 转接板资料（PCB V2.0） | [`docs/PCB-1.6寸AMOLED屏转接板V2.0.pdf`](./docs/PCB-1.6%E5%AF%B8AMOLED%E5%B1%8F%E8%BD%AC%E6%8E%A5%E6%9D%BFV2.0.pdf) |
| 板对板连接器规格（OK-14F024-04） | [`docs/OK-14F024-04.pdf`](./docs/OK-14F024-04.pdf) |

### 示例工程

- [ESP32-P4 ST7802 MIPI + LVGL9](./examples/esp32p4-idf5_st7802-mipi_esp-lvgl-port_lvgl9/)
- [ESP32-P4 LVGL9 + TE](./examples/with-te/esp32p4-idf5_st7802-mipi_lvgl9-common-demo/)
- [ESP32-P4 EAF player](./examples/eaf/esp32p4-idf5_st7802-mipi_lvgl9_esp-lv-eaf-player/)
- [ESP32-P4 ST7802 显示测试](./examples/display-touch-test/esp32p4-idf5_st7802-mipi-dsi/)
- [ESP32-P4 CST9220 触摸测试](./examples/display-touch-test/esp32p4-idf5_cst9220-i2c/)

## 购买链接

<p align="center">
  <a href="https://shop110742373.taobao.com/"><img alt="淘宝官方店铺" src="https://img.shields.io/badge/淘宝-官方店铺-FF6A00?style=for-the-badge" /></a>
  &nbsp;&nbsp;
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="速卖通官方店铺" src="https://img.shields.io/badge/速卖通-官方店铺-FF6A00?style=for-the-badge" /></a>
</p>

**国内（淘宝）**

- 店铺：[鱼鹰光电工厂店](https://shop110742373.taobao.com/)

**海外（AliExpress）**

- 店铺：[OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

## 技术支持

- 技术支持 / 产品咨询：<luyu@osptek.com>
- QQ 技术交流群：**985881096**
- 公司官网：<https://osptek.com/>

---

<p align="center"><sub>© 2026 OSPTEK 鱼鹰光电 · 本仓库资料采用 CC BY 4.0 许可</sub></p>

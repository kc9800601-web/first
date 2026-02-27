# 基于 Wio-Terminal 的种植大棚环境监测系统

本项目是用于监测大棚内实时环境数据的物联网终端系统，能够采集并展示关键的环境指标。

## 🛠️ 硬件清单
* 主控板：Wio-Terminal
* 传感器：Grove - SCD41 (二氧化碳、温度、湿度三合一传感器)

## ✨ 实现功能
* 实时读取 SCD41 传感器的 CO2 浓度 (ppm)。
* 实时读取当前环境的温度 (°C) 和相对湿度 (%)。
* 在 Wio-Terminal 的 LCD 屏幕上直观显示上述数据。

## 🚀 快速开始
### 1. 硬件连接
通过 Grove 接口将 SCD41 传感器连接到 Wio-Terminal 的 I2C 接口。

### 2. 软件依赖
在 Arduino IDE 的“库管理器”中，需要搜索并安装以下依赖库：
* `Sensirion I2C SCD4x` (用于驱动 SCD41 传感器)
* `TFT_eSPI` (Wio-Terminal 屏幕显示基础库，通常已内置)

### 3. 编译与烧录
1. 使用 USB-C 数据线将 Wio-Terminal 连接至电脑。
2. 在 Arduino IDE 中选择开发板为 "Seeeduino Wio Terminal"。
3. 验证代码无误后，点击“上传”将固件烧录至开发板。
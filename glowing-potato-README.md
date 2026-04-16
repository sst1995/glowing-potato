# 🎃 Glowing Potato

<!-- shields.io 徽章 -->

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Arduino%20%7C%20ESP32%20%7C%20Raspberry%20Pi-green.svg)
![Difficulty](https://img.shields.io/badge/difficulty-Medium-yellow.svg)
![Last Commit](https://img.shields.io/badge/last%20commit-April%202026-orange.svg)

---

## 📸 项目预览

<!-- 将你的效果图放到 images 目录，替换下方路径 -->

![Project Preview](images/preview.gif)
![Hardware Setup](images/hardware.jpg)

---

## 🌟 特性

- ✨ **智能控制** — 支持手机 APP / 语音 / Web 控制
- 🔋 **低功耗设计** — 待机电流 < 10μA
- 🌈 **RGB 灯效** — 1600 万色可调，多种动态模式
- 📱 **远程监控** — 实时状态上报，WiFi / 蓝牙双模
- 🔧 **模块化设计** — 易于扩展传感器和执行器

---

## 🛠 硬件清单

| 零件 | 数量 | 备注 |
|------|------|------|
| ESP32 开发板 | 1 | 或 Arduino Uno |
| WS2812B RGB LED | 8 | 环形或条形均可 |
| DHT11 温湿度传感器 | 1 | 可选 |
| 面包板 | 1 | 400孔 |
| 杜邦线 | 若干 | 母对母 |

---

## 📦 快速开始

### 硬件连接

```
ESP32 GPIO16  →  WS2812B DIN
ESP32 3.3V    →  WS2812B 5V
ESP32 GND     →  WS2812B GND
```

### 软件安装

```bash
# 克隆项目
git clone https://github.com/sst1995/glowing-potato.git
cd glowing-potato

# 安装依赖
npm install

# 编译上传
platformio run --target upload
```

### 配置 WiFi

编辑 `src/config.h`：

```cpp
#define WIFI_SSID "你的WiFi名称"
#define WIFI_PASSWORD "你的WiFi密码"
```

---

## 📁 项目结构

```
glowing-potato/
├── src/
│   ├── main.cpp          # 主程序入口
│   ├── led.cpp            # LED 控制逻辑
│   ├── wifi.cpp           # 网络连接
│   └── config.h           # 配置文件
├── images/                # 效果图片
├── schematic/             # 电路原理图
├── LICENSE
└── README.md
```

---

## 🎨 效果展示

| 模式 | 描述 |
|------|------|
| 🌙 呼吸灯 | 缓慢明暗变化，适合夜灯 |
| 🌈 彩虹 | 色彩渐变流动 |
| ⚡ 闪电 | 随机闪烁效果 |
| 🎵 音乐律动 | 跟随声音节奏跳动 |

---

## 📚 参考资料

- [FastLED 库文档](https://github.com/FastLED/FastLED)
- [ESP32 Arduino 教程](https://docs.espressif.com/)
- [Adafruit NeoPixel 指南](https://learn.adafruit.com/adafruit-neopixel-uberguide)

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

## 📄 许可证

清华小学 © 2026 sst1995

---



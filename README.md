# anycubic Mega Zero 2.0
[Marlin https://github.com/MarlinFirmware](https://github.com/MarlinFirmware)
[KlackEnder-Probe https://github.com/kevinakasam/KlackEnder-Probe](https://github.com/kevinakasam/KlackEnder-Probe)


# 中文说明
anycubic Mega Zero 2.0 Marlin-2.1.2.4 原厂主板固件,增加对 KlackEnder-Probe 的支持

## 固件修改
- 禁用启动屏幕显示
- 过热保护 热端: 260° 热床: 125 °
- 开启 KlackEnder Z探针支持
- Z探针替代 Z-MIN 限位开关
- "Z_MIN_PROBE_PIN" 定义为 29 (使用主板EXT-A2接口)
- 热床尺寸 225 * 225
- 使用 "AUTO_BED_LEVELING_BILINEAR" 网床调平
- 网床网格点数 6*6 (超过此数值程序会跑飞...)
- 开启 "LCD_BED_TRAMMING" 用于在手动调整床面时在床角之间移动 (A4纸调平)
- 开启 "Z_SAFE_HOMING" Z安全归位
- 温度预设 PLA 190° 60°
- 温度预设 PETG 230° 70°
- LCD界面语言 "en"
- 开启 "ASSISTED_TRAMMING" 探针四角调平
- 自定义菜单增加 "disable software endstops" 用于禁用软件限位来调整获得"Z-Offset"

**没有更多flash开启"PROBE_OFFSET_WIZARD"选项所以"Z-Offset"获取设置比较麻烦**

## KlackEnder-Probe 修改
- 修改 ProbeMount TabWidth 参数已适应amz2
- 重建 ProbeDock,ProbeRetainer 模型已适应amz2


# Instructions in English
---

**Firmware Modifications:**

- Disable startup screen display.
- Overheat protection: Hotend at 260°C, heated bed at 125°C.
- Enable KlackEnder Z probe support.
- Replace Z-MIN endstop switch with the Z probe.
- Define "Z_MIN_PROBE_PIN" as 29 (using the mainboard EXT-A2 interface).
- Bed size: 225 x 225 mm.
- Use "AUTO_BED_LEVELING_BILINEAR" for mesh bed leveling.
- Set the bed mesh grid to 6x6 points (going beyond this value may cause issues).
- Enable "LCD_BED_TRAMMING" to move between bed corners during manual bed leveling (similar to using A4 paper).
- Enable "Z_SAFE_HOMING" for safe Z-axis homing.
- PLA temperature presets: 190°C hotend, 60°C bed.
- PETG temperature presets: 230°C hotend, 70°C bed.
- Set LCD interface language to "en" (English).
- Enable "ASSISTED_TRAMMING" for four-corner bed leveling using the probe.
- Custom menu option added: "disable software endstops" to adjust "Z-Offset" without using additional flash memory.

---

**KlackEnder-Probe Modifications:**

- Adjusted ProbeMount TabWidth parameter to fit AMZ2.
- Rebuilt ProbeDock and ProbeRetainer models to accommodate AMZ2.
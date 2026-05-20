# 📝 记录：下载报错 "No Target Connected"

## 📅 时间

2026-05-20

## ❌ 问题描述

点击 Download 按钮后，提示无法连接芯片，但 ST-Link 灯是亮的。

## ✅ 解决方案

1. 检查杜邦线连接是否松动（特别是 SWDIO 和 SWCLK）。
2. 在 Keil 中点击 "Settings" -> "Flash Download"，勾选 "Reset and Run"。
3. **最终原因：** 开发板供电不足，更换 USB 口后解决。
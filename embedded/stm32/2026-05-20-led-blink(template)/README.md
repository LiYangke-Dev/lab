# 💡 [实验名称，如：STM32 GPIO点灯实验]

## 🎯 实验目标

- [ ] 掌握 [知识点，如：GPIO推挽输出配置]
- [ ] 学会使用 [工具，如：STM32CubeMX] 生成代码
- [ ] 实现 [现象，如：LED每隔1秒闪烁]

## 🛠️ 开发环境
- **硬件**: [如：STM32F103C8T6 核心板]
- **IDE**: [如：Keil uVision5]
- **库版本**: [如：HAL库 v1.8.0]



## 🛠️ 硬件连接

- LED正极 -> PA5
- LED负极 -> GND

## 📝 实验原理

> 简述原理：PA5引脚连接LED正极，输出低电平点亮，输出高电平熄灭。

## ⚙️ 关键代码
```c
// 核心逻辑代码片段
while (1) {
    HAL_GPIO_TogglePin(GPIOA, GPIO_PIN_5);
    HAL_Delay(500);
}
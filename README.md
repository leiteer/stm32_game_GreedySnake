# STM32F4 贪吃蛇游戏

基于STM32F407开发板实现的经典贪吃蛇游戏，具有精美的LCD显示界面和流畅的游戏体验。

## 主要功能

- 精美的主菜单界面
  - 动态的S形蛇图标
  - 游戏标题显示
  - 操作说明
![微信图片_20250110154647](https://github.com/user-attachments/assets/249f7e66-28ea-433d-9d01-21088d434165)

- 游戏功能
  - 流畅的蛇身移动
  - 实时分数显示
  - 食物随机生成
  - 碰撞检测
  - 游戏结束判定
![微信图片_20250110154659](https://github.com/user-attachments/assets/8e0e36e2-f5d6-47d8-a8a8-060fe5090662)

- 游戏结束界面
  - 显示最终得分
  - 一键返回主菜单
![微信图片_20250110154659](https://github.com/user-attachments/assets/4cff058c-32f2-45a2-bb49-bbee18b721e6)


## 硬件要求

- STM32F407开发板
- LCD显示屏（240x320）
- 按键模块：
  - KEY_UP
  - KEY0
  - KEY1
  - KEY2

## 操作说明

1. 主菜单界面
   - 按KEY0开始游戏

2. 游戏控制
   - KEY_UP：向上移动
   - KEY1：向下移动
   - KEY2：向左移动
   - KEY0：向右移动

3. 游戏结束后
   - KEY0：返回主菜单

## 开发环境

- Keil MDK 5
- STM32CubeMX
- ARM编译器

## 目录结构
STM32F4_Snake/

├── Core/

│ ├── Inc/

│ └── Src/

├── Drivers/

│ ├── Mydrivers/

│ │ ├── snake.c // 游戏核心代码

│ │ ├── snake.h // 游戏头文件

│ │ ├── lcd.c // LCD驱动

│ │ ├── lcd.h

│ │ ├── key.c // 按键驱动

│ │ └── key.h

│ └── STM32F4xx_HAL_Driver/

└── MDK-ARM/

## 编译说明

1. 使用Keil MDK打开项目
2. 编译整个项目
3. 下载到开发板

## 注意事项

- 确保LCD和按键模块正确连接
- 游戏区域为220x270像素
- 蛇的最大长度限制为100格
- 游戏速度可通过修改延时时间调整

## 版本历史

- v1.0.0 (2024-01-20)
  - 实现基础游戏功能
  - 添加主菜单界面
  - 完善游戏结束处理
  - 优化显示效果

## 作者

[leiteer](https://github.com/leiteer)

## 开源协议

MIT License

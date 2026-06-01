# 大鱼吃小鱼 HTML5 游戏 Spec

## Why
用户需要一个简单的 HTML5 大鱼吃小鱼小游戏，适合浏览器直接运行，无需额外依赖。

## What Changes
- 创建一个独立的 HTML5 游戏文件，包含 Canvas 渲染、游戏逻辑、玩家控制
- 使用纯 HTML/CSS/JavaScript 实现，无任何外部库
- 游戏支持键盘和触摸操作

## Impact
- 新增游戏文件：`/workspace/big-fish-eats-small-fish.html`

## ADDED Requirements

### Requirement: 游戏核心玩法
系统应提供一个大鱼吃小鱼的街机游戏，玩家控制一条鱼在海洋中移动，吃掉比自己小的鱼来成长，同时避开比自己大的鱼。

#### Scenario: 玩家吃小鱼
- **WHEN** 玩家控制的鱼碰到比自己小的鱼
- **THEN** 小鱼被吃掉，玩家分数增加，玩家体型略微增大

#### Scenario: 玩家被大鱼吃
- **WHEN** 玩家控制的鱼碰到比自己大的鱼
- **THEN** 游戏结束，显示最终分数

#### Scenario: 玩家成长
- **WHEN** 玩家吃掉多条小鱼后
- **THEN** 玩家体型逐渐增大，可以吃掉更大的鱼

### Requirement: 操作控制
系统应支持键盘方向键/WASD 控制鱼的移动，同时支持鼠标点击移动。

#### Scenario: 键盘控制
- **WHEN** 玩家按下方向键或 WASD
- **THEN** 鱼向对应方向移动

#### Scenario: 鼠标控制
- **WHEN** 玩家点击游戏区域
- **THEN** 鱼向点击位置移动

### Requirement: 游戏界面
系统应显示当前分数、玩家体型等级，以及游戏开始/结束界面。

#### Scenario: 游戏 HUD
- **WHEN** 游戏进行中
- **THEN** 屏幕显示当前分数和体型等级

#### Scenario: 游戏开始
- **WHEN** 页面加载完成
- **THEN** 显示开始界面，包含游戏说明和开始按钮

#### Scenario: 游戏结束
- **WHEN** 玩家被大鱼吃掉
- **THEN** 显示结束界面，包含最终分数和重新开始按钮

### Requirement: 鱼类生成
系统应持续生成不同大小的 NPC 鱼，以不同速度在屏幕中移动。

#### Scenario: NPC 鱼生成
- **WHEN** 游戏进行中
- **THEN** 持续从屏幕边缘生成不同大小的鱼，横穿屏幕

### Requirement: 视觉效果
系统应使用 Canvas 绘制简单的鱼形图案，不同大小的鱼有不同颜色。

#### Scenario: 鱼的外观
- **WHEN** 游戏渲染
- **THEN** 每种大小的鱼有独特颜色和形状，玩家鱼有特殊标识

# Tasks
- [x] Task 1: 创建 HTML 结构和游戏界面
  - [x] SubTask 1.1: 创建 HTML 文件骨架，包含 Canvas 元素
  - [x] SubTask 1.2: 实现游戏开始/结束界面 UI
  - [x] SubTask 1.3: 实现 HUD 显示（分数、体型等级）

- [x] Task 2: 实现玩家鱼的控制和渲染
  - [x] SubTask 2.1: 实现键盘方向键/WASD 控制
  - [x] SubTask 2.2: 实现鼠标点击移动
  - [x] SubTask 2.3: 绘制玩家鱼（Canvas 绘制鱼形）

- [x] Task 3: 实现 NPC 鱼系统
  - [x] SubTask 3.1: 实现 NPC 鱼生成逻辑（不同大小、速度）
  - [x] SubTask 3.2: 实现 NPC 鱼移动和屏幕边界处理
  - [x] SubTask 3.3: 绘制 NPC 鱼（不同颜色区分大小）

- [x] Task 4: 实现游戏核心逻辑
  - [x] SubTask 4.1: 碰撞检测（玩家与 NPC 鱼）
  - [x] SubTask 4.2: 吃小鱼逻辑（分数增加、体型增长）
  - [x] SubTask 4.3: 被大鱼吃逻辑（游戏结束）

- [x] Task 5: 完善游戏流程
  - [x] SubTask 5.1: 实现游戏开始/重新开始功能
  - [x] SubTask 5.2: 实现游戏循环和帧率控制
  - [x] SubTask 5.3: 优化视觉效果和用户体验

# Task Dependencies
- [Task 2] depends on [Task 1]
- [Task 3] depends on [Task 1]
- [Task 4] depends on [Task 2] and [Task 3]
- [Task 5] depends on [Task 4]

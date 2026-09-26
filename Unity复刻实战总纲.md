# Unity 复刻实战总纲

## 使用方式

本清单按玩法类型组织。所列项目均提供公开源码，但多数并非 Unity 工程；复刻时重点参考其玩法规则和系统设计，用 Unity/C# 独立实现一个较小的可玩版本。难度只是相对估计，默认不包含联网、完整美术或大量关卡。

| 类型 | 开源项目 | 建议的首个可玩版本 | 重点练习 | 难度 |
| --- | --- | --- | --- | --- |
| 益智／网格 | [2048 原版](https://github.com/gabrielecirulli/2048) | 4×4 棋盘、滑动合并、计分、结束判定 | 数组与网格、输入、UI、状态管理 | ★ |
| 2D 平台跳跃 | [SuperTux](https://github.com/SuperTux/supertux) | 移动、跳跃、踩敌人、收集物、单关卡 | 物理碰撞、角色手感、动画、关卡 | ★★ |
| 俯视角冒险／动作 RPG | [FreeDink](https://www.gnu.org/software/freedink/about)、[Flare](https://github.com/flareteam/flare-game) | 一张地图、近战攻击、两种敌人、道具 | 地图、战斗、AI、背包与数据配置 | ★★～★★★ |
| 俯视角射击／太空探索 | [Endless Sky](https://github.com/endless-sky/endless-sky) | 飞船转向与惯性、射击、敌机、升级 | 运动、弹道、生成、成长系统 | ★★ |
| 纵向卷轴射击 | [OpenTyrian](https://github.com/opentyrian/opentyrian) | 飞机移动、弹幕、敌人波次、Boss | 对象生成、碰撞、关卡节奏 | ★★ |
| Roguelike 地牢 | [Shattered Pixel Dungeon](https://github.com/00-Evan/shattered-pixel-dungeon) | 随机房间、回合移动、战斗、拾取物品 | 程序生成、回合制、物品系统 | ★★★ |
| 塔防／自动化 | [Mindustry](https://github.com/Anuken/Mindustry) | 路径刷怪、建塔、资源、波次 | 路径、目标选择、资源循环 | ★★★ |
| 回合制战棋 | [韦诺之战](https://github.com/wesnoth/wesnoth) | 网格移动、攻击范围、回合切换、简单 AI | 寻路、规则判定、回合状态 | ★★★ |
| 经营模拟 | [OpenTTD](https://github.com/OpenTTD/OpenTTD) | 建站、连接路线、运输货物、收入结算 | 模拟、经济循环、数据与 UI | ★★★★ |
| 3D 卡丁车竞速 | [SuperTuxKart](https://github.com/supertuxkart/stk-code) | 一辆车、一条赛道、计圈与检查点 | 3D 控制、相机、碰撞、计时 | ★★★ |
| 3D 第一人称射击 | [Xonotic](https://github.com/xonotic/xonotic) | 移动、瞄准、两把武器、靶场或简单敌人 | 角色控制、射线检测、武器与反馈 | ★★★ |
| 体素沙盒 | [Minetest Game](https://github.com/luanti-org/minetest_game)（运行于 [Luanti](https://github.com/luanti-org/luanti)） | 小地图、放置／破坏方块、物品栏 | 方块数据、网格生成、交互与存档 | ★★★★ |

## 推荐推进顺序

1. **2048**：先完成一个规则明确、规模可控的完整游戏。
2. **2D 平台跳跃**：练习 Unity 的碰撞、动画、相机和关卡制作。
3. **俯视角射击或动作 RPG**：根据兴趣选择，加入敌人和成长系统。
4. **战棋、塔防、竞速等**：在掌握前面的基础后，逐步处理更复杂的系统。

每个项目先实现表中的最小版本，完成试玩和复盘后再决定是否扩展。学习日志、计划日期和实际进度由仓库维护者持续更新。

## Unity 工程参考

如果希望直接研究 Unity/C# 项目，可参考 [Unity 版 2048](https://github.com/dgkanatsios/2048) 和 [Red Runner](https://github.com/BayatGames/RedRunner)。这些是引擎实现参考；上表中的经典项目主要用于研究玩法。

## 素材与许可

公开源码不等于所有图片、音乐、名称都能任意使用。发布复刻作品前，分别核对代码和素材许可；练习以自己的素材或许可明确的素材为宜。

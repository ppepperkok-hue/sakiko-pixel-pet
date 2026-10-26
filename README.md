<a id="top"></a>
<div align="center">

<img src="previews/states/idle.gif" alt="丰川祥子像素桌宠" width="128" />

# Sakiko Pixel Pet · 丰川祥子像素桌宠

<!-- moe-counter:start -->
<a href="https://github.com/journey-ad/Moe-Counter"><img src="https://count.getloli.com/get/@ppepperkok-hue.sakiko-pixel-pet?theme=asoul" alt="README views" width="360" /></a>
<br /><sub></sub>
<!-- moe-counter:end -->

*白衬衫、灰格裙、蓝灰长发，让日常服的祥子陪你工作。*

![Format](https://img.shields.io/badge/spritesheet-v2-a8b9eb)
![Frames](https://img.shields.io/badge/frames-73-8b9dc3)
![PNG](https://img.shields.io/badge/PNG-transparent-6c9a8b)
![Version](https://img.shields.io/badge/assets-1.0.0-d6aa60)
![Fan art](https://img.shields.io/badge/fan_art-unofficial-bb86b6)

**简体中文** · [English](README_EN.md)

</div>

---

## 目录

| 开始使用 | 进一步了解 |
| --- | --- |
| [✨ 内容](#features) | [🧩 文件与格式](#files) |
| [🎞️ 动作预览](#preview) | [🔍 校验结果](#validation) |
| [🚀 使用图集](#usage) | [⚠️ 已知边界](#limits) |
| [❓ 常见问题](#faq) | [📄 角色与素材说明](#notice) |

<a id="features"></a>
## ✨ 内容

这是以《BanG Dream! It's MyGO!!!!!》《BanG Dream! Ave Mujica》中的**丰川祥子**为原型制作的非官方像素风桌宠素材，面向 ChatGPT Work 的 Pets 工作流。

| 内容 | 说明 |
| --- | --- |
| **日常服造型** | 白色长袖衬衫、黑领结、灰格半身裙、白短袜和黑色玛丽珍鞋；没有面罩或手持道具。 |
| **九种基础动作** | 待机、向右跑、向左跑、招手、跳跃、失败反馈、等待回应、专注处理和复核，共 57 帧。 |
| **十六方向视线** | 从正上方开始顺时针排列，身体保持稳定，由头部和视线表达方向，共 16 帧。 |
| **透明 v2 图集** | `1536 × 2288` PNG，8 列、11 行，每格 `192 × 208`，73 个有效帧。 |
| **预览和来源** | 提供逐状态 GIF、整套动作 GIF / MP4、跳跃衔接预览、视线循环及选定的源动作条。 |

<a id="preview"></a>
## 🎞️ 动作预览

<div align="center">
<img src="previews/all-states.gif" alt="九种基础动作循环预览" width="384" />
<img src="previews/look-loop.gif" alt="十六方向视线循环预览" width="384" />
</div>

[下载 MP4 预览](previews/all-states.mp4) · [待机 → 跳跃 → 待机](previews/idle-jump-idle.gif) · [完整动作总览](previews/contact-sheet.png) · [方向检查图](previews/directions.png)

| 状态 | 图集行 / 帧数 | 预览 |
| --- | --- | --- |
| 待机 | 0 / 6 | [idle](previews/states/idle.gif) |
| 向右跑 | 1 / 8 | [running-right](previews/states/running-right.gif) |
| 向左跑 | 2 / 8 | [running-left](previews/states/running-left.gif) |
| 招手 | 3 / 4 | [waving](previews/states/waving.gif) |
| 跳跃 | 4 / 5 | [jumping](previews/states/jumping.gif) |
| 失败反馈 | 5 / 8 | [failed](previews/states/failed.gif) |
| 等待回应 | 6 / 6 | [waiting](previews/states/waiting.gif) |
| 专注处理 | 7 / 6 | [running](previews/states/running.gif) |
| 复核 | 8 / 6 | [review](previews/states/review.gif) |

这里的 `running` 是“正在处理任务”的状态名；实际移动使用 `running-right` 和 `running-left`。

<a id="usage"></a>
## 🚀 使用图集

**成品文件：[assets/sakiko-v2.png](assets/sakiko-v2.png)**

把这张原始 PNG 交给支持现有图集导入的 Pets 工作流，说明：

> 使用这张现成的 v2 图集创建自定义桌宠，保留原图，不重新生成角色或动作。

该工作流需要先验证图集，再上传并创建；需要显示新桌宠时再选中它。本次制作已通过 Pets 插件预检并成功创建。

> [!NOTE]
> 请使用原始 PNG，不要把预览 GIF、总览图或聊天截图当作图集上传。不同客户端开放的入口可能不同，本仓库提供的是素材包，不包含独立的 Windows 桌宠运行程序。

<a id="files"></a>
## 🧩 文件与格式

```text
assets/
└── sakiko-v2.png           最终透明图集
previews/
├── all-states.gif / .mp4  九种基础动作
├── look-loop.gif         十六方向视线
├── idle-jump-idle.gif     起跳与落地衔接
├── motion-stills.png      带时间的代表帧
├── contact-sheet.png     全图集总览
├── directions.png        方向检查图
└── states/               每种状态的 GIF
source/
├── canonical-idle.png    已确认的比例基准
├── animations/           九种动作的选定源图
└── look-directions/      四向基准与两条视线源图
validation/               公开校验摘要
manifest.json             格式、帧序和文件哈希
```

前九行从每行第一格开始使用，未使用的 15 个格子保持透明。第 9、10 行各使用 8 格：

```text
row 9:  000, 022.5, 045, 067.5, 090, 112.5, 135, 157.5
row 10: 180, 202.5, 225, 247.5, 270, 292.5, 315, 337.5
```

`000` 表示向上，`090` 向屏幕右侧，`180` 向下，`270` 向屏幕左侧。源动作条的洋红背景用于提取，成品图集已经去除背景并处理透明边缘。

<a id="validation"></a>
## 🔍 校验结果

| 检查 | 结果 |
| --- | --- |
| 格式与结构 | PNG / RGBA，`1536 × 2288`，73 个有效帧，未使用格透明，通过。 |
| 图集质量 | 基础动作帧数、图像边界、透明背景和方向位置检查通过。 |
| 跳跃 | 最高点相对落脚基线抬升 40 像素，落地与待机基线相差 1 像素。 |
| 视线方向 | 3 份独立盲审、14 对方向检查，严格多数结果全部通过。 |
| Pets 预检 | `valid: true`。 |
| 视频 | MP4 编码后解码检查通过，预览从最终 PNG 的实际格子裁取。 |

对应证据见 [validation/summary.json](validation/summary.json)。最终 PNG 的 SHA-256：

```text
d0f6201028d8db6d62d26abd9b405f611b91d19f19a485ca7f7d2b84407f86bb
```

<a id="limits"></a>
## ⚠️ 已知边界

- 这是经过多轮选择和修订的 AI 辅助同人素材，不是官方像素人设。
- `090 → 112.5` 与 `157.5 → 180` 的转头幅度比相邻角度明显；方向、人物比例与脚底定位检查通过，平滑度保留为已知视觉边界。
- 复核动作采用最终选定的第一版，幅度较轻。
- 校验覆盖当前图集和 Pets 创建流程，未覆盖所有客户端版本或其他桌宠引擎。

<a id="faq"></a>
## ❓ 常见问题

<details>
<summary><b>为什么下载后不能直接双击运行？</b></summary>

仓库提供的是动画图集与预览。需要由兼容该图集格式的 Pets 环境负责播放、拖拽和状态切换。

</details>

<details>
<summary><b>为什么源图是洋红色背景？</b></summary>

源动作条使用 `#FF00FF` 作为提取背景。实际使用 `assets/sakiko-v2.png`，它已经是透明背景。

</details>

<details>
<summary><b>“专注处理”为什么叫 running？</b></summary>

这是图集状态名称，表示任务执行中。对应动作是专注与思考，不是脚步跑动。

</details>

<a id="notice"></a>
## 📄 角色与素材说明

本项目是非官方同人创作。丰川祥子及《BanG Dream!》相关角色、名称和设定的权利属于各自权利人，本项目不代表官方授权或背书。仓库未声明通用开源许可证，详见 [NOTICE.md](NOTICE.md)。

## 🙏 鸣谢

- [BanG Dream! Ave Mujica 官方角色页](https://anime.bang-dream.com/avemujica/character/sakiko/) — 角色设定参考；官方立绘未收录在本仓库中。
- OpenAI ImageGen 与 Pets 工作流 — 图像生成、图集制作与预检。
- [astrbot_plugin_tavern](https://github.com/ppepperkok-hue/astrbot_plugin_tavern) — README 版式参考。

## 💬 反馈

欢迎通过 [Issues](https://github.com/ppepperkok-hue/sakiko-pixel-pet/issues) 反馈。请附上具体状态、帧序或方向，以及实际显示的截图，方便定位到对应素材。

<div align="center">

**[⬆ 回到顶部](#top)**

</div>

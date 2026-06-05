# 2026 World Cup Predictor / 2026 世界杯竞猜分析

> A single-file, offline-capable, framework-free web app for exploring the 2026 FIFA World Cup (48 teams, 12 groups, 72 group-stage matches) through data-driven schedule analysis, Monte-Carlo qualification/title simulations, an interactive knockout bracket, and a money-free score-prediction game.
>
> 单文件、可离线、无框架的纯前端网页应用，围绕 2026 世界杯（48 队、12 小组、72 场小组赛）提供数据驱动的赛程分析、蒙特卡洛出线/夺冠模拟、交互式淘汰赛对阵树，以及一个不涉及金钱的比分竞猜游戏。

[English](#english) · [中文](#中文)

---

## English

### Features
- **Groups** — all 12 groups with "group of death" detection
- **Schedule** — 72 matches with win/draw/loss probability bars and venue weather hints
- **Simulation** — per-group qualification & top-spot odds from a full-tournament Monte Carlo (default 6000 runs)
- **Deep analysis** — title-odds Top 12, group difficulty, history-continuity read, knockout drills, contender profiles
- **Knockout** — interactive bracket (32→16→8→4→2→1), zoom/pinch, drag to predict
- **Score prediction** — two scoring modes + a streak challenge, points only (no odds, no money)
- **Bilingual** — built-in 中文 / English toggle (top-right)
- **Privacy-first** — notes & predictions stored only in your browser `localStorage`; nothing is uploaded

### Run
Just open `index.html` in any modern browser. No build step, no install, no server. Fully offline except an optional weather lookup (silently degrades on failure).

### Tech
- Single HTML file: inline CSS + vanilla JavaScript, no framework, no bundler
- Math models: Elo-style win/draw/loss with Gaussian draw correction; Poisson score model (independent)
- Optional live weather via the free, key-less [Open-Meteo](https://open-meteo.com) API (CC BY 4.0)

### Disclaimer
This is an **entertainment & analysis tool, not an official source and not a betting tool**. Team ratings are manual estimates, not official rankings; all probabilities are mathematical inference, not predictions. The score game uses points only — no real odds, payouts, or wagering.

### License
[MIT](LICENSE)

---

## 中文

### 功能
- **小组一览** — 12 个小组，自动识别死亡之组
- **赛程分析** — 72 场比赛，胜/平/负概率条 + 场馆天气提示
- **出线模拟** — 完整赛事蒙特卡洛（默认 6000 次）统计各组出线与头名概率
- **深度分析** — 夺冠概率 Top 12、小组难度、历史延续性、淘汰赛演练、竞争者阵容研判
- **淘汰赛** — 交互式对阵树（32→16→8→4→2→1），可缩放/捏合、拖拽预测
- **比分竞猜** — 两套计分规则 + 连续命中挑战，纯积分（无赔率、无金钱）
- **中英双语** — 右上角一键切换
- **隐私优先** — 备注与竞猜仅存浏览器 `localStorage`，不上传任何数据

### 运行
用任意现代浏览器打开 `index.html` 即可。无需构建、安装或服务器。除可选的天气查询外完全离线（查询失败时静默降级）。

### 技术
- 单 HTML 文件：内联 CSS + 原生 JavaScript，无框架、无打包器
- 数学模型：Elo 思路胜平负 + 高斯平局修正；独立的泊松比分模型
- 可选实时天气来自免密钥的 [Open-Meteo](https://open-meteo.com) API（CC BY 4.0）

### 免责声明
本程序是**娱乐与分析工具，非官方信息源、非投注工具**。球队评分为人工估计、非官方排名；所有概率均为数学推演，不代表预测。比分竞猜仅积分，无真实赔率、奖金或下注。

### 许可
[MIT](LICENSE)

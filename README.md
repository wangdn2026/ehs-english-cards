# EHS 英语 · 口袋书

> 「安全五点半」英语训练营 · 配套素材仓库  
> 专为 E. H. S.（环境、健康、安全）从业者打造的职场英语场景化学习

「安全五点半」是 **GET YOU·AI 试驾** 旗下面向 EHS 从业者的英语训练品牌。本仓库存放每期配套的听读页、词卡、跟读素材等全部网页化资产。

**在线访问**：https://wangdn2026.github.io/ehs-english-cards/

---

## 项目亮点

- **场景化教学**：每期围绕一个 EHS 真实场景（巡检 / PPE / 化学品 / 应急 / JHA 等）
- **三种学习方式**：听读页（系统学习）+ 分级跟读卡（碎片练习）+ 翻翻页词卡（打印随身）
- **每周双场直播**：
  - **周一 19:45** — EHS 英语训练营（主课）
  - **周三 21:15** — 线上英语口语练习（视频号「安全五点半」）
- **音频配套**：每卷独立 MP3（含 part1 / part2 / part3 / full）

---

## 内容索引

| 卷 | 主题 | 状态 |
|---|---|---|
| Vol.00 | 开播词 Program Opening | ✅ |
| Vol.01 | 上岗前 Before Starting Work | ✅ |
| Vol.02 | 现场巡检 Site Inspection | ✅ |
| Vol.03 | 穿戴 PPE Wearing PPE | ✅ |
| Vol.04 | 化学品安全 Chemical Safety | ✅ |
| Vol.05 | 事故报告 Incident Reporting | ✅ |
| Vol.06 | 应急演练 Emergency Drill | ✅ |
| Vol.07 | JHA 工作危害分析 Job Hazard Analysis | ✅ |
| Vol.08 D1 | 员工报告不安全状态 · Dialogue 1 | ✅ |
| Vol.08 D2 | 员工报告不安全状态 · Dialogue 2 | ✅ |
| Vol.09 | 工厂危害识别 Workplace Hazards | 🟡 即将上线 |

---

## 仓库结构

```
ehs-english-cards/
├── index.html                  # 主页（GitHub Pages 入口）
├── listener_volXX_*.html       # 听读页（每卷独立，含音频同步）
├── graded_volXX_*.html         # 分级跟读卡（L1 / L2 / L3）
├── card_volXX_*.html           # 入口卡（SAFETY 时钟 + 星级目录）
├── flipbook_N_*.html           # 翻翻页词卡（A4 打印折页）
├── player_*.html               # 单页词卡播放器
├── dialogue_volXX_*.json       # 对话原始数据（metadata + parts + lines）
├── phrase_pool_volXX_*.json    # 词卡原始数据（phrases + part_summary）
└── *.mp3                       # 音频素材（part1 / part2 / part3 / full）
```

---

## 本地预览

纯静态文件，本地启动 HTTP 服务即可：

```bash
# Python 3
python3 -m http.server 8000

# 或 Node.js
npx http-server
```

打开 http://localhost:8000 访问主页。

---

## 部署

`main` 分支推送即自动部署（GitHub Pages 默认配置）：

```bash
git -c http.version=HTTP/1.1 push origin main
```

---

## 缩略词规则

所有正文中的 `EHS` 必须转写为 **`E. H. S.`**（字母间加句号停顿），避免 TTS 吞音。

---

## 维护说明

- 每期新卷按 `项目文档/样板模板/` 下的模板生成
- `dialogue_volXX_*.json` 含 metadata（volume / topic / speakers / key_phrases）+ parts（lines）
- `phrase_pool_volXX_*.json` 含 phrases（id / phrase / translation / example / scenario / image_hint）
- 听读页 / 卡片 / 翻翻页 / 音频时长等元数据需保持一致

---

## 关联项目

- **试听体验**：[wangdn2026/ehs-trial](https://github.com/wangdn2026/ehs-trial) — EHS 英语 1 分钟试听（三个独立入口）

---

## 团队与直播时间

- 主讲：Frank（38 年英文兼职教学）
- 运营：唐老师
- 助教：[王冬妮](mailto:wangdn@coze.email)

| 时间 | 内容 |
|---|---|
| 周一 19:45 | EHS 英语训练营（主课） |
| 周三 21:15 | 线上英语口语练习（视频号「安全五点半」） |

---

## 品牌归属

本仓库是 **GET YOU·AI 试驾** 旗下「安全五点半」英语训练营的素材仓库。

| 品牌 | 角色 | 视觉 |
|---|---|---|
| GET YOU·AI 试驾 | 母品牌 | 天青 + 暖橙 + 深炭灰 |
| 安全五点半 | 子品牌 | 安全黄 + 警示红 + 深底色 + 仪表盘 LOGO |

Slogan：**传统行业普通人用 AI 告别杂活**

---

*Made by 王冬妮 · GET YOU·AI 试驾*
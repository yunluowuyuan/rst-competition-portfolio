# 徐浩渊 · 个人主页 | Personal Portfolio

> 工业工程 × 航空航天 × AI —— 交叉方向探索者的工程实践集

一个零外部框架依赖的个人主页，内嵌两枚由 HTML5 Canvas 独立开发的交互游戏（《星河战机》《坦克大战》），以真实工程实践展示「AI 协同开发」工作流与系统化学习方法论。

## 📌 个人简介

- **姓名**：徐浩渊
- **方向**：工业工程 × 航空航天 × 人工智能（交叉探索）
- **教育**：南昌航空大学 · 工业工程（2026.09 入学）
- **特点**：以"计划—执行—审计—纠偏"（PDCA）闭环驱动自我迭代；借助 AI 协同编程将创意快速落地为可运行产品。
- **联系**：nfxhyspace0714@163.com

## ✨ 核心技术栈与工程亮点

| 类别 | 技术/方案 |
|------|-----------|
| 渲染 | HTML5 Canvas 独立游戏引擎（主循环 / 粒子系统 / 对象池） |
| 逻辑 | `requestAnimationFrame` 固定步长帧循环、帧率无关 `dt` 驱动 |
| 碰撞 | AABB 轴对齐包围盒 + 瓦片地图网格化判定 |
| 音频 | WebAudio 程序化音效（零音频资源文件） |
| 主题 | CSS 变量双主题（深空 / 明亮）+ `prefers-color-scheme` 自适应 |
| 架构 | 单文件纯净架构，原生 HTML/CSS/JS，零构建、零依赖 |
| 协同 | AI 协同开发（Prompt Engineering 模块化拆解 → 审查 → 合并） |

**核心亮点**

- 🎮 **独立 Canvas 游戏引擎**：不依赖 Phaser / PixiJS 等任何第三方库，从零实现渲染循环、实体系统、碰撞检测、粒子特效与 UI 状态机。
- 🎧 **WebAudio 程序化音频**：音效实时合成，游戏目录不含任何音频素材文件。
- 🌓 **深浅色双主题**：CSS 变量 + 系统级适配，深空科幻与明亮简洁一键切换。
- ♿ **无障碍设计**：语义化标签、ARIA、键盘 Tab 导航、弹窗焦点圈定。
- 📱 **全端适配**：375px ~ 1920px 无横向溢出，触屏与键盘双输入。
- 🔗 **GitHub Pages 就绪**：全站相对路径引用，可直接部署于二级目录。

## 📁 项目目录结构

```
.
├── index.html                 # 个人主页（数据层 / 渲染层 / 交互层三段式单文件架构）
├── plane.html                 # 《星河战机》COSMIC STRIKER · Canvas 空战游戏
├── tank.html                  # 《坦克大战》经典核心框架 · Canvas 游戏
├── README.md
└── assets/
    └── images/
        └── certs/             # 25 张 AI 认证证书图片（kebab-case 规范命名）
            ├── cert-ai-junior-2026.jpg
            ├── cert-ai-senior-2026.jpg
            ├── cert-ai-university-01.png
            └── cert-misc-01.png …
```

> 命名规范：所有素材均为 `kebab-case` 英文命名，无中文、空格与特殊字符，保证跨平台与静态部署兼容性。

## 🚀 本地预览

纯静态站点，无需安装任何依赖，三种方式任选：

**方式一 · 直接双击**

```bash
# 双击打开 index.html 即可浏览主页（Canvas 游戏在主页内弹窗运行）
index.html
```

**方式二 · 本地静态服务器（推荐，避免 file:// 限制）**

```bash
# Python
python -m http.server 8080
# 或 Node.js
npx serve .
# 浏览器访问 http://localhost:8080
```

**方式三 · 单独体验游戏**

```bash
# 直接打开对应游戏页
plane.html    # 《星河战机》
tank.html     # 《坦克大战》
```

## 🌐 GitHub Pages 部署

全站采用相对路径引用，支持直接部署到二级目录。

1. 将本仓库推送至 GitHub；
2. 仓库 `Settings → Pages → Deploy from a branch`，选择 `main` / `main branch`（根目录）；
3. 等待部署完成，访问：

```
https://<username>.github.io/<repository>/
```

> ⚠️ 占位说明：以上链接中的 `<username>` 与 `<repository>` 为占位符，请替换为你实际的 GitHub 账号与仓库名。

## 📄 许可证

本项目仅供学习与竞赛交流使用，保留所有权利（All Rights Reserved）。

---

**致谢**：本项目中的两枚游戏均以「人类定义目标与边界，AI 生成实现，人类负责审查、调试与验收」的 AI 协同开发模式完成。

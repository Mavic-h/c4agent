# C4Agent

**可见、可控的多智能体协作工作台（macOS）**

让 Codex、Claude、Gemini 等真实 CLI 智能体，在同一个项目里协同工作。

---

## ⬇️ 下载

[**下载最新版 (.dmg · Apple Silicon)**](https://github.com/Mavic-h/c4agent/releases/latest/download/C4Agent-1.2.0-arm64.dmg)

> 适用于 Apple Silicon（M1/M2/M3…）的 Mac，约 99 MB，免费。

也可以在 [Releases 页面](https://github.com/Mavic-h/c4agent/releases/latest) 查看所有版本。

---

## 📦 安装说明（重要）

本应用未经 Apple 公证签名，首次打开会被系统拦截。请按任一方式打开：

**方式一（推荐）**
1. 双击下载好的 `.dmg`，把 **C4Agent** 拖进「应用程序」。
2. 打开时若提示「已损坏 / 无法验证开发者」，**右键点击 App 图标 → 打开**，再在弹窗里点「打开」。

**方式二（更彻底）**
打开「终端」，执行：
```bash
xattr -cr /Applications/C4Agent.app
```
之后即可正常双击打开。

> 这是 macOS 对未签名应用的正常安全提示，并非软件损坏。

---

## ✨ 核心特性

- **可见** — 每个智能体的运行过程实时呈现：谁在执行、谁在等待、谁需要确认，一目了然。
- **可控** — 为每个智能体分配角色、提示词、模型与独立工作区，显式编排协作。
- **真实** — 每个面板跑的都是真实 CLI 进程，不是模拟套壳。
- **独立工作区** — 每个智能体可拥有独立的 git worktree，安全并行。

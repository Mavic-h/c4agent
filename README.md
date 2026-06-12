# C4Agent

**可见、可控的多智能体协作工作台（macOS）**

让 Codex、Claude、Gemini 等真实 CLI 智能体，在同一个项目里协同工作。

---

## ⬇️ 下载

[**下载最新版 (.dmg · Apple Silicon)**](https://github.com/Mavic-h/c4agent/releases/latest/download/C4Agent-arm64.dmg)

> 适用于 Apple Silicon（M1/M2/M3…）的 Mac，约 99 MB，免费。

也可以在 [Releases 页面](https://github.com/Mavic-h/c4agent/releases/latest) 查看所有版本。

---

## 📦 安装说明（重要）

本应用做了 **ad-hoc 签名**（不会再报「已损坏」），但因未做 Apple 付费公证，**首次打开需要一次性放行**：

1. 双击 `.dmg`，把 **C4Agent** 拖进「应用程序」。
2. 首次打开任选一种放行方式：
   - **右键**点 App 图标 → **打开** → 弹窗里再点「打开」；
   - 或 **系统设置 → 隐私与安全性**，下拉到底点 **「仍要打开 / Open Anyway」**。
3. 之后即可正常双击使用，不再提示。

**最省事的一行命令**（打开「终端」执行，直接去掉隔离标记）：

```bash
xattr -dr com.apple.quarantine /Applications/C4Agent.app
```

> 这是 macOS 对非 App Store / 未公证应用的正常安全机制，并非软件问题。若需要"双击零提示"，需用 Apple 开发者账号做公证签名。

## ✨ 核心特性

- **可见** — 每个智能体的运行过程实时呈现：谁在执行、谁在等待、谁需要确认，一目了然。
- **可控** — 为每个智能体分配角色、提示词、模型与独立工作区，显式编排协作。
- **真实** — 每个面板跑的都是真实 CLI 进程，不是模拟套壳。
- **独立工作区** — 每个智能体可拥有独立的 git worktree，安全并行。

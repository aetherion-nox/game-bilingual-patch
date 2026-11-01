# 游戏双语补丁 Skill

一个用于 Codex 等支持 `SKILL.md` 的智能体的技能，指导制作、扩展和修复游戏双语本地化补丁，让两种语言在字幕、提示和界面中同时呈现。

它强调可靠的文本配对、格式与控制码保留、按实际界面调整排版，以及区分构建、安装和实机验证。本仓库提供工作方法，不包含现成游戏补丁或游戏资源；支持范围取决于具体游戏。

## 安装

将本仓库完整克隆到 Codex 的技能目录（或将整个目录复制到该目录）：

```bash
git clone https://github.com/aetherion-nox/game-bilingual-patch.git ~/.codex/skills/game-bilingual-patch
```

在 Windows 上，该目录通常为 `%USERPROFILE%\.codex\skills\game-bilingual-patch`。安装后重新启动 Codex，使技能列表刷新。

## 使用

在 Codex 中说明游戏、需要的两种语言及主辅语言，并提出制作或修复双语补丁的需求；也可明确指定 `game-bilingual-patch`。实际实施需要相应游戏文件、版本信息和必要授权。

## 文件

- [SKILL.md](SKILL.md)：技能入口与核心工作流程。
- [排版与取舍](references/layout-and-fallback.md)：布局和回退策略。
- [验证与交付](references/verification-and-delivery.md)：验证与交付要求。
- [agents/openai.yaml](agents/openai.yaml)：Codex 技能显示信息。

本技能用于两种语言同时显示；按键切换语言的场景请使用 `game-language-toggle-mod` 技能。


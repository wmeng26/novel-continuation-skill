# novel-continuation — 小说续写 Skill

[ZCode](https://zcode.ai) 技能：续写任意小说、网文、同人。先提取原文"设定档案"（视角、文风指纹、人物口癖、世界观规则、悬置点），按需联网查证原著设定与写作技法（含 GitHub 资源、短语接龙取原文），再规划情节节拍、无缝续写，最后对照质量清单自检。

## 文件结构

```
.agents/skills/novel-continuation/
├── SKILL.md                       # 触发描述 + 五步工作流
└── references/
    ├── craft-checklist.md         # 自检清单（拼接/文风/人物OOC/逻辑/钩子）
    └── web-research-guide.md      # 联网查证手册（短语接龙法、工具回退梯）
```

## 在新电脑上安装

- **工作区级（推荐）**：clone 本仓库后，用 ZCode 打开该文件夹即可自动发现，无需其他操作。
- **用户级（全机器可用）**：把 `novel-continuation` 文件夹复制到 `~/.agents/skills/` 下。

注意：同名 skill 用户级优先于工作区级，建议只维护本仓库这一份，改动后 `git push`，其他机器 `git pull` 同步。

## 日常迭代

修改 SKILL.md 或 references 后：

```bash
git add . && git commit -m "更新说明" && git push
```

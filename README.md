# 崔走召文风 Skill（cuizouzhao-novelist）

> 东北民俗志怪 · 说书人腔 · 命运主题 · 崔氏统一宇宙

## 这是什么

一个可复用的 **Agent Skill**：基于崔走召《我当阴阳先生的那几年》《我当鸟人的那几年》《三途志》三部曲**全本**蒸馏出的**叙事操作系统**，让 AI 能以崔氏文风**原创小说、续写、改写**，并能做**文风分析**。

本 skill 不复制原文、不摘抄段落，只提炼「怎么写」的可执行规则。

## 快速开始

把本仓库当作一个 Agent Skill 使用：

```text
用崔走召的风格写一个东北乡村的灵异短篇
```

```text
用「日常→渗人」的节奏，续写下面这段……
```

```text
分析下面这段文字，给出崔氏文风的修改建议
```

主文件是 `SKILL.md`，Agent 会读取它作为创作守则。更细的技法库在 `references/`，按需查阅。

## 目录结构

```text
cuizouzhao-novelist/
├── SKILL.md                        # 主技能文件（叙事操作系统，入口）
├── README.md                       # 本说明
├── references/                     # 技法库（按需读取）
│   ├── worldbuilding.md            # 世界观构建技法（地府官僚/秘境/魔神法则）
│   ├── style-guide.md              # 文风语言技法（说书人腔/口语/唱词体/工业恐怖）
│   ├── structure.md                # 结构技法（倒计时/伪重置/因果闭环/心愿清单/群像收束）
│   ├── characters-theme.md         # 人物塑造与主题技法
│   ├── crossbook-universe.md       # 崔氏统一宇宙（跨书闭环时间线）
│   ├── samples.md                  # 样本库（民俗招式/说书套话/收官金句/道具/秘境）
│   └── kelivo-pack.md              # Kelivo 三合一配置（系统提示词+指令注入+世界书）
└── worldbook/                      # （可选）RikkaHub 可导入世界书 JSON
    └── cuizouzhao-worldbook.json   # 崔氏文风世界书（20 词条，与 kelivo-pack.md C 部分对应）
```

## 触发场景

- 原创：写一个崔氏风格的都市灵异/东北民俗志怪故事
- 续写：按崔氏笔法续写章节
- 改写：把一段普通文本改成崔氏文风
- 分析：用崔氏规则诊断文本并给修改建议
- Kelivo 导入：系统提示词+指令注入+世界书三合一（`references/kelivo-pack.md` + `worldbook/cuizouzhao-worldbook.json`）

## 版本

- v1.0：基于已蒸馏进度（yingyang 96% / santu 67% / niaoren 32%）
- v2.0：yingyang 全书读毕，命运母题与前世轮回线落定
- v3.0：三部曲全本读完（100%），补全三书结局线、收官技法模型、跨书闭环时间线；新增可导入 JSON
- **v3.1：整合 cuizouzhao-skill 全部内容（三书调性对照/写作工作流/质检清单/参数建议/Kelivo 三合一配置），本仓库为唯一维护源**

## 许可

参考同类型 skill 仓库惯例，本仓库使用 MIT License（如需其他许可请提 Issue）。

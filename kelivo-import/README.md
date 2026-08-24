# Kelivo 导入包 · 崔走召文风（v3.1）

本目录是 Kelivo 可直接导入的三件套（依据 cuizouzhao-skill 最终版整合）。

## 文件清单

```text
kelivo-import/
├── 系统提示词.txt                 # ① 复制粘贴到助手设置
├── 指令注入/
│   ├── B1_语言硬标记.txt          # ② 多选导入（文件名=标题，内容=prompt）
│   ├── B2_民俗土招与世界观铁律.txt
│   ├── B3_情绪弧线与节奏.txt
│   ├── B4_结构引擎.txt
│   └── B5_质检交付与禁用词.txt
└── worldbook/
    └── cuizouzhao-worldbook.json  # ③ 世界书直接导入（20 词条）
```

## 导入步骤（iOS）

1. **系统提示词**：GitHub 网页打开 `系统提示词.txt` → 全选复制 → Kelivo「助手 → 编辑 → 系统提示词」粘贴保存。
2. **指令注入**：把 `指令注入/` 里 5 个 txt 文件逐个下载到「文件」App → Kelivo「设置 → 指令注入」→ 右上角导入图标 → 多选这 5 个文件（标题会带 .txt，可自行改名）。
3. **世界书**：下载 `worldbook/cuizouzhao-worldbook.json` → Kelivo「设置 → 世界书」→ 右上角导入图标 → 选该 JSON（导入后记得在对应助手的世界书里勾选启用）。

## 说明

- 指令注入导入时标题=文件名（含 .txt），可在 Kelivo 内长按改名；如需分组，编辑时填分组名。
- 世界书关键词大小写不敏感子串匹配、OR 触发；priority 降序；position=AFTER_SYSTEM_PROMPT（并入系统提示）。
- 参数建议：创作 temperature 0.8 / top_p 0.9；润色 0.5–0.55 / 0.85。

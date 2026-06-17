# scientific-humanization

用于中文科研文本的 humanization：把论文、综述、基金、项目书、技术方案、答辩、课程讲稿、PPT 讲稿和投资人科研表达改得更像专业作者或讲师本人在说，同时保护事实、术语、数字、引用、图表编号和证据强度。

这个 skill 的目标不是同义词替换，也不是把文本改得更“高级”，而是让表达更自然、更清楚，并且不把科学结论说过头。

## 适用场景

- 用户说“别 AI 味”“人一点”“别太官方”
- 用户要求“像我讲的”“去模板腔”“改顺但别改事实”
- 科研 PPT、课程讲稿或答辩稿需要更像真人口播
- 论文正文、项目书或技术方案需要降低空泛表达、强化证据边界

## 安装

把本仓库克隆到本地后，将整个目录复制到 Codex skills 目录：

```bash
git clone https://github.com/TashanGKD/scientific-humanization.git
cp -R scientific-humanization ~/.codex/skills/
```

Windows PowerShell 示例：

```powershell
git clone https://github.com/TashanGKD/scientific-humanization.git
Copy-Item -Recurse -Force .\scientific-humanization $env:USERPROFILE\.codex\skills\
```

## 目录结构

```text
SKILL.md
README.md
```

## 工作原则

- 先锁定事实，再调整表达。
- 先改论证顺序，再改句子。
- 保留数字、单位、引用、图表编号、模型名、数据集和实验条件。
- 相关性不能写成因果，趋势不能无依据写成显著。
- 对讲稿可以更口语，对论文正文要更保守。

## 输出风格

默认直接给可用版本。文本风险高时，可以按以下结构输出：

```text
主要问题：
保留事实：
改后正文：
仍需确认：
```

`仍需确认` 只放会影响事实或证据边界的事项，不放泛泛建议。

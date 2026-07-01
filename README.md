# Virtual Character Realism Design

Skill ID：`virtual-character-realism-design-zh`

中文名：虚拟角色拟真设计

这是一个面向中文虚拟角色创作的 skill。它的目标不是把角色卡字段填满，而是帮助作者把角色做得更像人：有稳定底色，有选择顺序，有关系变化，有欲望、羞耻、身体反应、误解、停顿和不体面，也能被分流写入角色卡、世界书、记忆、预设或状态规则。

## 适合做什么

- 从模糊灵感整理出可长期互动的角色。
- 修订已有角色卡，让角色少一点标签感。
- 把设定分流写入角色核心、世界书、记忆、预设和关系规则。
- 设计用户画像、关系变化、亲密与身体性处理方式。
- 检查角色扮演是否 AI 腔、模板化、抢用户或过早开高潮戏。

## 目录结构

```text
README.md
LICENSE
NOTICE.md
THIRD_PARTY_LICENSES.md
virtual-character-realism-design-zh/
  SKILL.md
  agents/
    openai.yaml
  references/
    theory.md
    workflow.md
    question-bank-36.md
    question-bank-108.md
    question-bank-260.md
    writing-targets.md
    dual-characters.md
    anti-ai-tone.md
    cases.md
```

## License

MIT License. Copyright (c) 2026 cOkieeman.

Third-party license notices are collected in [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md).

## 作为 Codex Skill 使用

把 `virtual-character-realism-design-zh/` 这个文件夹放到 Codex 可读取的 skills 目录，或在支持 skill 仓库导入的环境中指向本仓库。

使用时可以这样说：

```text
Use $virtual-character-realism-design-zh 帮我把这个角色想法整理成更像人的角色系统。
```

或：

```text
Use $virtual-character-realism-design-zh 帮我把这段设定分流成角色卡、世界书、记忆和预设。
```

## 作为普通 AI 提示文件使用

如果目标平台不支持 Codex skill，可以先把 `SKILL.md` 给 AI 阅读，再按任务补充对应 reference：

- 理解理论和术语：`references/theory.md`
- 决定工作流程：`references/workflow.md`
- 快速追问：`references/question-bank-36.md`
- 完整建模：`references/question-bank-108.md`
- 深度抽题：`references/question-bank-260.md`
- 写入角色卡、世界书、记忆、预设：`references/writing-targets.md`
- 多角色关系和防串味：`references/dual-characters.md`
- 去 AI 腔：`references/anti-ai-tone.md`
- 示例和反例：`references/cases.md`

不要一次性把所有 reference 都塞给模型。先判断任务，再读取对应文件。

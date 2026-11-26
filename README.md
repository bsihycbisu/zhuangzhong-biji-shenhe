# 代理笔记审核 Skill

给小红书代理稿做审核的 WorkBuddy 技能。

**只审两件事：产品事实不能错，篇内逻辑要自洽。** 不改稿、不代笔，输出「结论 / 问题清单 / 整体判断」。

针对庄重读书会（中文名著、古文观止）两款产品，内含 Brief 全文、课表、91 本书目、常见错法对照。

---

## 安装

### 方式一：让 AI 自己装（推荐）

把这句话发给你的 AI：

```
git clone https://github.com/bsihycbisu/zhuangzhong-biji-shenhe 到临时目录，然后把 SKILL.md 和 references/ 整个复制到 ~/.workbuddy/skills/笔记审核/
（Windows 是 C:\Users\你的用户名\.workbuddy\skills\笔记审核\）
复制完告诉我装好了，并列出装进去的文件。
```

### 方式二：手动装

```bash
git clone https://github.com/bsihycbisu/zhuangzhong-biji-shenhe
```

把仓库里的 `SKILL.md` 和 `references/` 放进：

```
C:\Users\你的用户名\.workbuddy\skills\笔记审核\
├── SKILL.md
└── references\
```

或者直接下载 `note-review-skill.zip`，解压到 `.workbuddy\skills\` 下即可。

> 注意：`SKILL.md` 必须**直接**在 `笔记审核` 文件夹里，不能再套一层。

### 验证

重开一个会话，问：「你有哪些审稿相关的技能？」

然后直接丢稿子说「审一下这篇」，它应该按「结论 / 问题清单 / 整体判断」三段回你。

---

## 内容

| 文件 | 用途 |
|---|---|
| `SKILL.md` | 触发条件、审核流程、事实摘要、91 本书目 |
| `references/brief-cn.md` | 中文名著 Brief 全文（71 KB） |
| `references/brief-gu-wen.md` | 古文观止 Brief 全文（25 KB） |
| `references/brief-si-da.md` | 四大名著 Brief（⛔ 暂停审核，仅存档） |
| `references/kecheng-cn.md` | 中文名著课表：级别 / 书目 / 出版社 / 属性 |
| `references/kecheng-gu-wen.jpg` | 古文观止 40 节排期与十大单元原图 |

**核对顺序**：先查 `SKILL.md` 里的「产品事实速查」→ 查不到翻 `references/` 原文 → 原文也没有，标「待确认」。

---

## 更新

课程数字变了（换书目、改课时、调口径），只改 `SKILL.md` 的「六、产品事实速查」这一节，其他文件不用动。

# QA 报告:{APP_NAME}

| 字段 | 值 |
|------|-----|
| **日期** | {DATE} |
| **URL** | {URL} |
| **分支** | {BRANCH} |
| **提交** | {COMMIT_SHA} ({COMMIT_DATE}) |
| **PR** | {PR_NUMBER} ({PR_URL}) 或 "—" |
| **等级** | Quick / Standard / Exhaustive |
| **范围** | {SCOPE 或 "Full app"} |
| **耗时** | {DURATION} |
| **访问页面数** | {COUNT} |
| **截图数** | {COUNT} |
| **框架** | {DETECTED 或 "Unknown"} |
| **索引** | [所有 QA 运行](./index.md) |

## 健康分:{SCORE}/100

| 类别 | 分数 |
|------|------|
| 控制台 | {0-100} |
| 链接 | {0-100} |
| 视觉 | {0-100} |
| 功能 | {0-100} |
| UX | {0-100} |
| 性能 | {0-100} |
| 无障碍 | {0-100} |

## 最该修复的 3 件事

1. **{ISSUE-NNN}:{title}** —— {一句话描述}
2. **{ISSUE-NNN}:{title}** —— {一句话描述}
3. **{ISSUE-NNN}:{title}** —— {一句话描述}

## 控制台健康

| 错误 | 次数 | 首次出现 |
|------|------|----------|
| {error message} | {N} | {URL} |

## 汇总

| 严重程度 | 数量 |
|----------|------|
| Critical | 0 |
| High | 0 |
| Medium | 0 |
| Low | 0 |
| **总计** | **0** |

## 问题

### ISSUE-001:{Short title}

| 字段 | 值 |
|------|-----|
| **严重程度** | critical / high / medium / low |
| **类别** | visual / functional / ux / content / performance / console / accessibility |
| **URL** | {page URL} |

**描述:** {哪里出错,期望 vs 实际。}

**复现步骤:**

1. 进入 {URL}
   ![Step 1](screenshots/issue-001-step-1.png)
2. {操作}
   ![Step 2](screenshots/issue-001-step-2.png)
3. **观察:** {哪里出问题}
   ![Result](screenshots/issue-001-result.png)

---

## 已应用的修复(如适用)

| 问题 | 修复状态 | 提交 | 改动文件 |
|------|----------|------|----------|
| ISSUE-NNN | verified / best-effort / reverted / deferred | {SHA} | {files} |

### 修复前后证据

#### ISSUE-NNN:{title}
**修复前:** ![Before](screenshots/issue-NNN-before.png)
**修复后:** ![After](screenshots/issue-NNN-after.png)

---

## 回归测试

| 问题 | 测试文件 | 状态 | 描述 |
|------|----------|------|------|
| ISSUE-NNN | path/to/test | committed / deferred / skipped | 描述 |

### 延期的测试

#### ISSUE-NNN:{title}
**前置条件:** {触发该 bug 的初始状态}
**操作:** {用户执行的动作}
**期望:** {正确行为}
**为何延期:** {原因}

---

## 发布就绪度

| 指标 | 值 |
|------|-----|
| 健康分 | {before} → {after} ({delta}) |
| 发现问题数 | N |
| 已修复 | N (verified: X, best-effort: Y, reverted: Z) |
| 已延期 | N |

**PR 摘要:** "QA 发现 N 个问题,修复 M 个,健康分 X → Y。"

---

## 回归(如适用)

| 指标 | 基线 | 当前 | 变化 |
|------|------|------|------|
| 健康分 | {N} | {N} | {+/-N} |
| 问题数 | {N} | {N} | {+/-N} |

**自基线以来已修复:** {list}
**自基线以来新增:** {list}

# CIE 文学题库第二轮定点修复报告

## 修改文件

- `backups/index.before-targeted-fix.html`
- `backups/question_bank.before-targeted-fix.json`
- `work/question_bank.json`
- `outputs/index.html`
- `docs/LEARNING_ARCHITECTURE.md`
- `docs/PREDICTION_DESIGN.md`
- `docs/QUESTION_AUDIT.md`
- `docs/LEARNING_ARCHITECTURE_CHANGELOG.md`
- `IMPLEMENTATION_REPORT.md`
- `TARGETED_FIX_VALIDATION.md`

## 数据规模

- 题目总数：57
- id 新增：0
- id 删除：0
- core：20
- variation：28
- teacher-extension：9

## 特殊处理

- `fortress-gao-fang-attitude`：保留招揽、控制、切割三段主结构；新增两条 supplementaryEvidence，完整保存改版前证据、location、章节和检索词。
- `saffi-love`、`water-symbol`、`hospital-environment`、`water-contrast`、`fortress-fang-su-relationship`：不新增题目，显示统一无 direct variation 模块。
- `fortress-fang-father-character`、`fortress-fang-mother-character`：确认教师拓展归属，needsManualReview=false。

## Validation 结果

详细逐项结果见 `TARGETED_FIX_VALIDATION.md`。

## 项目运行方式

直接打开 `outputs/index.html`，或访问 GitHub Pages 地址。

## 页面模式

- 学生模式：默认启用，默认只显示 core，可切换 variation，教师拓展默认隐藏。
- 完整论证模式：显示 core 与 variation 的完整 PEEL，可展开补充证据。
- 教师／拓展模式：显示全部 57 题、分层信息和教师备注。


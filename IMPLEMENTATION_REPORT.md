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

- 默认页面：直接显示全部 57 道题的简洁大题库。
- 题库：按作品或关键词浏览题目，进入 Thesis 与 PEEL 详情。
- 母题匹配：恢复原版文本匹配入口。
- 真题预测：保留历年真题与预测方向。
- 随机抽题：从当前题库自由抽题。

## UI 回退与冻结

- `outputs/index.html` 已按 `backups/index.before-learning-architecture.html` 恢复为简洁大题库界面。
- 默认首页恢复为题库、母题匹配、真题预测、随机抽题，以及四部作品筛选。
- 默认列表直接显示全部 57 道题，统计文案为“共 57 道题目”。
- 学习模式切换、学习层级筛选、教师拓展筛选、进度、掌握状态和复杂学习引导已从默认页面移除。
- 题目详情恢复以 Thesis 和 PEEL 为主体；题干下仅保留一行“答题重点”。
- `supplementaryEvidence` 未删除，已以紧凑的“补充证据（改版前保留材料）”显示在详情页主体段之后。
- 本次只修改 HTML、CSS 和前端渲染逻辑，未修改 `work/question_bank.json`、题目 ID、顺序或任何文学内容。

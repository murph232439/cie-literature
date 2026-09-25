# Learning Architecture Changelog

修改日期：2026-09-25

## 新增字段完整清单

| 字段 | 用途 |
|---|---|
| learningLevel | 标记 core、variation 或 teacher-extension |
| studyPriority | 标记必背、高频变式或拓展 |
| parentQuestionId | variation 与教师拓展指向对应 core |
| doNotMemorizeSeparately | 标记变式与拓展不单独背全文 |
| questionFocus | 用学生可理解的句子说明题目真正要求 |
| socraticQuestions | 审题前引导学生思考 |
| notAsking | 明确常见跑题方向 |
| threePartPlan | 给出三段结构和可模仿起句 |
| commonMistakes | 列出错误、原因和修正方法 |
| summary | 30 字内概括本题逻辑 |
| studentNote | 给出复习提示或教师拓展说明 |
| supplementaryEvidence | 保存改版前被重组替代但仍须保留的补充证据 |
| answerRoutes | 同一题包含两种可选对象时提供分路线 |

## 分层变更

- core：20 题
- variation：{counts["variation"]} 题
- teacher-extension：{counts["teacher-extension"]} 题
- 所有 variation 与 teacher-extension 的 parentQuestionId 均指向有效题目。

## Point 重排与类型更正

- `fortress-parallel`：第三段 Point 改为明确回答平行关系的对照作用。
- `fortress-gao-fang-attitude`：按招揽、降级控制、解聘切割重组三阶段。
- `hospital-intellectual`：类型由“人物关系”更正为“人物与环境冲突”。

## Gao 题补充证据保留

- `fortress-gao-fang-attitude.supplementaryEvidence` 长度固定为 2。
- 第一项保留原先关于“容易对付”和改聘副教授的完整证据与第六章定位。
- 第二项保留原先关于增加英文课、把方鸿渐作为可调度劳动力的完整证据与第七章定位。
- 当前三个主 Point 的 evidence 均未删除。

## 学生模式新增模块

- 核心题底部显示“我会换一种问法考你”。
- 存在 direct variation 时逐项展示变式。
- 没有 direct variation 时显示统一兜底复习模块。
- 完整 PEEL 与补充证据默认折叠，学生点击后展开。

## 教师模式新增模块

- 教师模式显示全部 57 题及 learningLevel、studyPriority、parentQuestionId、studentNote 和 needsManualReview。
- 两道家庭人物题确认不再视为未分类缺口。
- 无 direct variation 的兜底模块额外显示“可在后续题库扩展中添加 direct variation。”

## 五道无 direct variation 的核心题

`saffi-love`、`water-symbol`、`hospital-environment`、`water-contrast`、`fortress-fang-su-relationship` 未虚构新题，统一显示暂未配置直接变式的复习说明。

## 两道遗漏家庭人物题最终确认

原始分层清单漏列两题。经补充分层：
- 方遯翁题归入“方鸿渐人物与家庭背景”教师拓展；
- 方老太太题归入“婚姻围城与家庭关系”教师拓展。
这两项已获确认，不再视为未分类缺口。

## 人工复核项

- `fortress-group-portrait`：教师拓展题，普通考试复习不必优先。
- `saffi-enlightenment-revolution`：教师拓展题，普通考试复习不必优先。
- `water-1930s-ecology`：教师拓展题，普通考试复习不必优先。
- `water-discourse-tension`：教师拓展题，普通考试复习不必优先。
- `hospital-dual-luping`：教师拓展题，普通考试复习不必优先。
- `fortress-new-women-portrait`：教师拓展题：比较五位女性，不要用“纯洁”或“心机”作道德标签。
- `fortress-old-women-choices`：教师拓展题：人物、家庭和婚恋结构同时涉及，不作为普通学生的必背题。


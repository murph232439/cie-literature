# Learning Architecture Changelog

- 修改日期：2026-09-25T20:50:47+08:00
- 原题数：57
- 原始备份：`backups/index.before-learning-architecture.html`
- 原始题库备份：`backups/question_bank.before-learning-architecture.json`

## Learning Levels

- 《围城》：共 29 题；必背 8；高频变式 16；教师拓展 5
- 《莎菲女士的日记》：共 9 题；必背 4；高频变式 4；教师拓展 1
- 《水》：共 9 题；必背 4；高频变式 3；教师拓展 2
- 《在医院中》：共 10 题；必背 4；高频变式 5；教师拓展 1

## 逐题分层

- fortress-tang-relationship：core；parentQuestionId=None
- saffi-character：core；parentQuestionId=None
- saffi-awakening：core；parentQuestionId=None
- saffi-psychology：variation；parentQuestionId=saffi-diary-form
- saffi-love：core；parentQuestionId=None
- water-symbol：core；parentQuestionId=None
- water-change：core；parentQuestionId=None
- water-hero：variation；parentQuestionId=water-change
- water-theme：core；parentQuestionId=None
- hospital-luping：core；parentQuestionId=None
- hospital-growth：core；parentQuestionId=None
- hospital-environment：core；parentQuestionId=None
- hospital-intellectual：variation；parentQuestionId=hospital-individual-collective
- fortress-fang：core；parentQuestionId=None
- fortress-satire：core；parentQuestionId=None
- fortress-marriage：core；parentQuestionId=None
- fortress-parallel：variation；parentQuestionId=fortress-fang
- saffi-loneliness：variation；parentQuestionId=saffi-awakening
- saffi-diary-form：core；parentQuestionId=None
- water-contrast：core；parentQuestionId=None
- water-wangdabao：variation；parentQuestionId=water-change
- hospital-group：variation；parentQuestionId=hospital-individual-collective
- hospital-gas：variation；parentQuestionId=hospital-growth
- hospital-ending：variation；parentQuestionId=hospital-growth
- fortress-diploma：core；parentQuestionId=None
- fortress-intellectuals：core；parentQuestionId=None
- fortress-metaphor：variation；parentQuestionId=fortress-satire
- fortress-group-portrait：teacher-extension；parentQuestionId=fortress-intellectuals
- fortress-language-satire：variation；parentQuestionId=fortress-satire
- fortress-concrete-balance：variation；parentQuestionId=fortress-satire
- saffi-imperfect-vanguard：variation；parentQuestionId=saffi-character
- saffi-awakening-tragedy：variation；parentQuestionId=saffi-awakening
- saffi-enlightenment-revolution：teacher-extension；parentQuestionId=saffi-awakening
- water-intellectual-stance：variation；parentQuestionId=water-theme
- water-1930s-ecology：teacher-extension；parentQuestionId=water-theme
- water-discourse-tension：teacher-extension；parentQuestionId=water-theme
- hospital-individual-collective：core；parentQuestionId=None
- hospital-dual-luping：teacher-extension；parentQuestionId=hospital-luping
- hospital-growth-useful：variation；parentQuestionId=hospital-growth
- fortress-sun-character：variation；parentQuestionId=fortress-marriage
- fortress-tang-character：variation；parentQuestionId=fortress-tang-relationship
- fortress-gao-songnian-character：variation；parentQuestionId=fortress-education-system-satire
- fortress-li-meiting-character：variation；parentQuestionId=fortress-intellectuals
- fortress-fang-father-character：teacher-extension；parentQuestionId=fortress-fang
- fortress-fang-mother-character：teacher-extension；parentQuestionId=fortress-marriage
- fortress-su-wenwan-character：variation；parentQuestionId=fortress-tang-relationship
- fortress-zhao-xinmei-character：variation；parentQuestionId=fortress-parallel
- fortress-new-women-portrait：teacher-extension；parentQuestionId=fortress-tang-relationship
- fortress-old-women-choices：teacher-extension；parentQuestionId=fortress-marriage
- fortress-education-system-satire：core；parentQuestionId=None
- fortress-zhao-sun-view：variation；parentQuestionId=fortress-sun-character
- fortress-gao-fang-attitude：variation；parentQuestionId=fortress-education-system-satire
- fortress-fang-leaves-university：variation；parentQuestionId=fortress-intellectuals
- fortress-travel-social-problems：variation；parentQuestionId=fortress-education-system-satire
- fortress-diploma-social-package：variation；parentQuestionId=fortress-diploma
- fortress-baoxia-relationship：variation；parentQuestionId=fortress-fang
- fortress-fang-su-relationship：core；parentQuestionId=None

## 结构校正

- `fortress-tang-relationship`：Point 顺序固定为苏文纨先贬低唐晓芙、再向唐晓芙提供方鸿渐旧事，最后写双方性格与误会如何导致分手。
- `fortress-gao-fang-attitude`：thesis、Points、Evidence 与 Explain 统一为高松年从招揽、降级到解聘的态度变化，主体始终为高松年。
- `fortress-parallel`：第三段 Point 明确回答平行关系的对照作用，并同时回扣人物塑造与社会环境。
- `fortress-diploma`：学习路径固定为爱情、事业、婚姻三个层面，再总结学历崇拜与身份包装的讽刺。
- `fortress-zhao-sun-view`：三段均以赵辛楣为观察主体，依次写照料与避嫌、警惕、订婚后的受限提醒。
- `fortress-fang-leaves-university`：三段按职业基础、校内环境和取消续聘形成原因链。
- `fortress-baoxia-relationship`：重点改为鲍小姐的现实主动性如何触发方鸿渐的虚荣、轻信与自我想象。
- `fortress-fang-su-relationship`：三段统一写方鸿渐的欣赏、暧昧享受、拖延伤害与责任逃避。
- `hospital-environment`：三段固定为现实处境、环境对人物行动的压迫、专业理想与组织现实的矛盾。
- `hospital-intellectual`：类型由人物关系改为人物与环境冲突。
- `fortress-old-women-choices`：题干改为旧式家庭与婚姻关系如何影响方鸿渐的婚恋选择。
- `fortress-new-women-portrait`：学生提示明确要求比较婚恋、名誉、阶层与社会限制，不使用道德标签。

## 分类口径说明

- 需求示例列出《围城》3 道教师拓展题，但题库原有 29 道《围城》题，其中 `fortress-fang-father-character` 与 `fortress-fang-mother-character` 也属于理论跨度较大的人物拓展题。
- 根据“不删除题目”的约束，这两题保留为 `teacher-extension`，因此《围城》教师拓展实际为 5 题。

## 仍需人工复核

- `saffi-enlightenment-revolution`：启蒙与革命语境需要外部分析背景。
- `water-1930s-ecology`：涉及1930年代上海文学生态。
- `water-discourse-tension`：涉及个性话语与革命话语理论。
- `fortress-old-women-choices`、`fortress-new-women-portrait`：群像跨度大，需人工复核男女角色与社会关系表述。

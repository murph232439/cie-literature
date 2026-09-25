# UI Rollback Validation

- 回退基准：`backups/index.before-learning-architecture.html`
- 当前站点文件：`outputs/index.html`
- 题目总数：57
- 验证结果：12/12 PASS

## 恢复与原版一致的元素

- 恢复顶部主导航：题库、母题匹配、真题预测、随机抽题。
- 恢复四部作品筛选：全部、《围城》、《莎菲女士的日记》、《水》、《在医院中》。
- 恢复大题库题卡列表，默认直接显示全部 57 道题。
- 恢复题卡的作品、题型、标题、题干和打开答题页按钮。
- 恢复详情页的 Thesis、Point、Evidence、Explain、Link 主体结构。
- 恢复搜索、母题匹配和随机抽题。
- 保留题干下的一行轻量“答题重点”。
- 保留 Gao 题的“补充证据（改版前保留材料）”内容。

## 已隐藏或移除的复杂 UI

- 学生模式／完整论证模式／教师模式切换。
- learningLevel、studyPriority、parentQuestionId 的页面展示。
- 核心题、变式题、教师拓展题的列表筛选。
- 无直接变式和母题关系的复杂大模块。
- 学习进度、掌握状态、每日任务、薄弱题和学习路线。
- needsManualReview、审校与题库映射等内部字段。

## 逐项验收

| 序号 | 验收项 | 结果 | 证据 |
|---|---|---|---|
| 1 | 默认首页视觉和信息层级接近改版前备份 | PASS | 恢复原版导航、筛选和题卡结构；浏览器测量默认列表为 57 张题卡 |
| 2 | 首页是完整大题库，不是学习路径或任务系统 | PASS | 默认页面不存在学习模式切换、进度、掌握状态或任务入口 |
| 3 | 可以自由浏览全部 57 道题 | PASS | 默认列表显示 57 道题 |
| 4 | 作品筛选正常 | PASS | 《围城》29、《莎菲女士的日记》9、《水》9、《在医院中》10 |
| 5 | 搜索正常 | PASS | 搜索“方鸿渐”返回 28 道相关题 |
| 6 | 随机抽题正常 | PASS | 成功抽题并显示“看论点与原文定位”按钮 |
| 7 | 题目详情以 Thesis + PEEL 为主体 | PASS | 详情显示中心论点、Point、Evidence、Explain、Link；Gao 题主体段和补充证据均可见 |
| 8 | 默认页面不显示学习层级、进度、掌握状态、母题映射等复杂系统 | PASS | DOM 可见文本中无 learningLevel、parentQuestionId、学习进度或掌握状态 |
| 9 | 不显示“共 54 道母题” | PASS | 当前显示“共 57 道题目” |
| 10 | 当前 57 题及其内容没有变化 | PASS | 题库 ID 顺序一致；`work/question_bank.json` 的 SHA256 与操作前一致 |
| 11 | 控制台无 JavaScript 报错 | PASS | error/warn 日志为空 |
| 12 | 390px 移动端无明显横向溢出 | PASS | viewport、body 和 document scrollWidth 均为 390，主内容溢出项为 0 |

## 未修改的数据文件及 SHA256

- `work/question_bank.json`
  - `2f53d0f00eec2e9952fe011975421433352ea6bdb80563cd4190d0c9314ab105`
- `backups/index.before-learning-architecture.html`
  - `aae1c26b25f3719ecda585673b0508a9593568d38195871e00c79e8e7fa5ebc3`
- `backups/question_bank.before-learning-architecture.json`
  - `9f9001ce10c24ad806350fdb469f20f6505e16c75e0d59c8217e0325f1dc6eba`

## 最终结论

UI 已恢复为简洁大题库形式，57 道题和全部文学内容保持不变。

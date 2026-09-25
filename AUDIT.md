# CIE Literature Question Bank Audit

Date: 2026-09-25

Current exported data: 57 questions, 171 points.

Machine audits completed with zero blocking issues:

- Point abstraction
- Explain support
- Causal chain
- Stage coverage
- Page format
- Evidence blocking checks
- Past-paper primary mapping

## Modified entries

### `fortress-tang-relationship`

- Original problem: `thesis` began with Su Wenwan slandering Tang Xiaofu to Fang Hongjian, but Point 1 began with Su showing Fang's letters to Tang. The paragraph order contradicted the thesis.
- Fix: reordered Point 1 and Point 2.
- Final order:
  1. Su Wenwan slanders Tang Xiaofu to Fang Hongjian.
  2. Su Wenwan shows Fang Hongjian's letters, old relationships, marriage arrangement, and diploma rumors to Tang Xiaofu.
  3. The breakup is completed by Tang Xiaofu's absolute standard of love and Fang Hongjian's refusal to explain.
- Removed the incorrect claim that Su Wenwan telephoned while Tang was already on the line and caused the final misunderstanding.
- Added classroom page 56 for Su Wenwan's direct slander to Fang Hongjian.

### `fortress-gao-fang-attitude`

- Original problem: the middle point claimed Gao Songnian did not care whether Fang Hongjian could teach English, while the evidence shows Gao asking about Fang's English ability.
- Fix: the point now states that Gao checks the ability first, then treats Fang as an available teaching resource according to staffing needs.
- Fixed `chain.who` values for all three points to `高松年`.

### `fortress-zhao-sun-view`

- Added a dedicated question for the past-paper topic `赵辛楣对孙柔嘉有哪些看法`.
- The previous default link opened `赵辛楣与方鸿渐`, which did not answer the question.

### `fortress-fang-leaves-university`

- Added a dedicated causal question for `方鸿渐离开三闾大学的原因`.
- The causes are divided into weak professional positioning, unstable departmental status, and Gao Songnian's politically framed non-renewal.

### `fortress-travel-social-problems`

- Added a dedicated question for `前往三闾大学的一路艰难反映出当时的哪些社会问题`.
- Covers unequal access to transportation, abuse of military privilege, and profiteering from scarce medicine.

### `fortress-diploma-social-package`

- Added classroom records on the fake diploma, the shame-covering metaphor, Zhou family packaging, `点金银行`, and the impersonal resume formula.

### `fortress-baoxia-relationship`

- Added classroom records on Bao Xiaojie's pragmatic background, the fiancé comparison, and the fiancé reveal as narrative irony.

### `fortress-fang-su-relationship`

- Added a dedicated question on Fang Hongjian's ambiguous attraction to Su Wenwan, his avoidance of a decision, and the eventual abrupt confrontation.

### `hospital-luping`

- Revised the middle explanation so it no longer claims lack of social experience from evidence that only proves conflict.
- Added direct evidence for insufficient worldliness and failure to observe others' reactions.

### `hospital-group`

- Rebuilt the group portrait into three categories: patients/residents, hospital staff, and lay management.
- Removed unsupported claims that the evidence did not prove.
- Added the specific staff categories requested: doctors' wives, short-term trained nurses, and service workers.

## Pending exact-version verification

The following classroom page mappings remain marked as classroom-record locations rather than verified printed-book page numbers:

- `fortress-tang-relationship`, stage 前: classroom page 56
- `fortress-diploma-social-package`, stages 前, 中, 后: classroom pages 10 and 29
- `fortress-baoxia-relationship`, stages 前, 中, 后: classroom pages 13, 14, and 22
- `fortress-fang-su-relationship`, stages 前, 中, 后: classroom page 24

These mappings display `课堂记录已定位；待统一版本逐字核验` and are not presented as verified `bookPage` values.

## Functional verification

The generated page was opened in the browser and checked:

- Question card: `苏文纨的挑拨与感情破裂` opened the same title and question.
- Paragraph order: Point 1 is Su Wenwan slandering Tang Xiaofu to Fang Hongjian; Point 2 is Su Wenwan showing Fang's letters and history to Tang Xiaofu.
- Search: `点金银行` returned the two expected diploma-related questions.
- Filter: selecting `《水》` returned 9 questions and removed the 《围城》 questions.
- Random draw: clicking the draw button produced a question and exposed the `看论点与原文定位` action.
- Past-paper navigation: `赵辛楣对孙柔嘉有哪些看法？请举例分析。` opened `赵辛楣对孙柔嘉的看法`, not `赵辛楣与方鸿渐`.

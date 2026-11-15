# Lesson Kit Design Skill · 教材包設計 Skill

**by Youth Impact Taiwan 青年啟航協會 (YIT)**

一個給 Claude 用的 skill，把 YIT 課程設計團隊的教材設計流程打包起來：從系列規劃、課綱與課本調查、大綱、教案、簡報、練習設計，到查證與品質檢查。Claude 負責調查、提選項和起草，設計者做決定。讓 YIT 成員和任何教育工作者都能用同一套方法，做出**志工拿到就能教**的雙語教材包。

A Claude skill that packages Youth Impact Taiwan's curriculum design process — series planning → curriculum research → outline → lesson plan → slides → practice design → verification and review, with Claude proposing options and the designer deciding — so YIT members and any educator can build bilingual, volunteer-ready lesson kits the same way.

---

## 這個 skill 會做什麼 What it does

- 先確認課程類型：系列性（先定系列大綱）或單元性
- 對新手友善：每個問題都說明為什麼問、不確定時怎麼想，並附預設值；附名詞小辭典
- 先讓你客製需求：課堂長度（預設 60 分鐘）、年級、練習形式、學生背景、是否接大地遊戲
- 課綱與課本調查：各年級在學校學過什麼，決定 A 版怎麼設計、B 版要簡化到哪裡（先設計 A 版，再簡化成 B 版）
- 大綱分版本迭代（v0.1, v0.2…），每一版列出需要你決定的事項
- 練習先列候選讓你挑選組合，檢查不超綱，排好難度順序和時間不夠時的退路
- 查證事實與例子、避開爭議、檢查教案／簡報／卡片／學習單是否一致
- 教案九大段：基本資料卡（含前後課連結）、學習目標、核心單字（標註字表來源）、逐頁指引（目標／中英引導句／方法／預期反應）、預期提問、變通方案、物品清單
- 簡報骨架：每頁的文字、畫面與可直接貼到 AI 繪圖／簡報工具的 prompt
- 練習至少佔一半：學習單（靜態、紙筆記憶）和／或活動練習（動態、肢體記憶，例如肢體遊戲、卡牌、Kahoot）
- 教案格式條件：中文一律標楷體、低年級全部加注音（建議用符合「注音IVS字型規格」的字嗨注音標楷，破音字可用讀音選擇工具設定；字型需自行下載）
- 輸出 .docx + .pdf；簡報依你習慣的工具，提供你喜歡的模板讓 AI 模仿
- 大地遊戲（G）另有獨立流程
- 品質 checklist：練習是否過半、時間是否可行、程度是否適合等

## 核心設計原則 Principles

1. **教案先於簡報** Lesson plan before slides
2. **練習一定超過一半** Practice is always >50% of the lesson (aim 60–70%) — 寧可少教、不要塞爆
3. **先查學生在學校學過什麼** Research what school has already taught before designing
4. **一條主線，只教需要的** One storyline; teach only what it needs
5. **不超綱** Practise only what was taught
6. **跨年級只用全部年級都學過的概念** Mixed-grade lessons only use concepts every grade has learned
7. **遊戲建立在教案上** Games build on lessons; game rules are taught in their own session

## 安裝 Install

### Claude.ai / Claude app
1. 下載這個 repo（Code → Download ZIP）
2. 把 `skills/lesson-kit-design` 資料夾單獨壓縮成 `lesson-kit-design.zip`
3. 在 Claude 的設定中找到 Skills，上傳這個 zip（需要你的方案／組織有開啟 skills 功能）

### Claude Code
```bash
git clone https://github.com/chanelhwung94-glitch/lesson-plan-design.git
cp -r lesson-plan-design/skills/lesson-kit-design ~/.claude/skills/
```

### 做成 Claude Project（不用安裝 skill 也能用）Use as a Claude Project
1. 建立一個新的 Claude Project
2. 把 `skills/lesson-kit-design/` 裡的檔案上傳到 Project 知識庫（有自己的字表也一起上傳）。上傳後資料夾結構可能不見，沒關係，Claude 會用檔名找到對應的檔案
3. 把 [`project-instructions.md`](project-instructions.md) 的內容貼到 Project 的指示欄位

## 使用方式 Usage

直接跟 Claude 說你要做的課，例如：

> 幫我設計一堂給 4–6 年級的雙語課，主題是動物的家，60 分鐘，志工來教，之後會接大地遊戲。

> Design a 40-minute Basic lesson for grades 1–3 on world festivals, with a worksheet.

> 幫我用品質 checklist 檢查這份教案。

## 不是 YIT 成員？ Not from YIT?

流程是通用的。代號、檔名、品牌（logo、配色）等團隊格式放在 `references/house-style-template.md`，裡面用 YIT 的代號與檔名系統當範例，填入你們自己的規範即可。

The process is general. Team conventions (level codes, file names, branding) live in one file — `references/house-style-template.md`, pre-filled with YIT's code system as an example. Fill in your own and everything else still works.

## 結構 Structure

```
skills/lesson-kit-design/
├── SKILL.md                     # workflow 流程
├── references/
│   ├── lesson-plan.md           # 教案
│   ├── slides.md                # 簡報
│   ├── worksheet.md             # 學習單
│   ├── intake-questions.md      # 需求設定的提問（附為什麼問）
│   ├── glossary.md              # 名詞小辭典
│   ├── curriculum-research.md   # 課綱與課本調查
│   ├── practice-design.md       # 練習設計（候選選單、遊戲、Kahoot）
│   ├── verification.md          # 查證、爭議與一致性
│   ├── scaffolding.md           # 系列性課程的連貫
│   ├── quality-checklist.md     # 品質檢查
│   ├── ground-game.md           # 大地遊戲
│   ├── output-format.md         # 輸出格式（docx+pdf、簡報模板）
│   ├── zhuyin.md                # 注音字型
│   └── house-style-template.md  # 團隊格式（自行填寫）
└── templates/                   # 空白範本
```

## 授權 License

[CC BY 4.0](LICENSE) — 歡迎使用、修改、分享（包括商業用途），請標註 Youth Impact Taiwan。字型、字表、課本等第三方資料不在此授權範圍內，請依各自的授權使用。

## 聯絡 Contact

Youth Impact Taiwan 青年啟航協會 · [youthimpacttaiwan.com](https://youthimpacttaiwan.com)
歡迎開 issue 或 pull request 分享你的改良。 Issues and pull requests welcome.

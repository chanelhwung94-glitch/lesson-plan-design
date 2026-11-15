# Lesson Plan Design Skill · 教案設計 Skill

**by Chanel from Youth Impact Taiwan**

一套「無痛」的教材設計方法，專門給**沒有教學經驗的人**。把它裝進你的 AI 助理，帶著一個主題來，AI 就會一路問你問題、解釋為什麼、提供選項讓你決定，最後交給你一整包**別人拿到就能直接教**的教材。

A painless way to design teaching materials, made for **people with no teaching experience**. Add it to your AI assistant, bring a topic, and the AI will guide you — asking the right questions, explaining why, offering options for you to choose — until you have a complete lesson kit **anyone can pick up and teach**.

---

## 適合誰 Who it's for

- **有想法，但不知道怎麼變成一堂課的人**：腦中有想教的主題或點子，卻不知道從哪裡開始、怎麼變成可以直接拿去教的教材
- **第一次設計教材的人**：志工、助教、營隊工作人員、想教點什麼的大學生。不需要教育背景
- **想讓團隊用同一套方法設計的人**：讓每一位成員做出來的教材格式一致、品質穩定，新成員也能很快上手
- **任何學科、任何年齡都可以用**：預設是台灣國小的雙語英文課，但進階版／初階版怎麼分、教什麼主題，都由你決定

- **People with an idea but no idea where to start**: you know what you want to teach, but not how to turn it into a lesson you can actually teach
- **First-time designers**: volunteers, teaching assistants, camp staff, students who want to teach something. No teaching background needed
- **Team leads** who want everyone on the team to design the same way — consistent format, steady quality, quick onboarding for new members
- **Any subject, any age**: the default is bilingual English lessons for Taiwanese elementary schools, but you decide the topic and how to split advanced and basic levels

## 你會得到 What you get

**設計過程中 While you design**
- 🧭 一開始就幫你釐清需求：時間、學生、場地、設備，每一題都告訴你為什麼要問，不知道怎麼答也有預設值
- 🗺️ 想做一系列的課？先幫你排好每一堂的主題和難度，一課接一課往上
- 🔍 幫你查學生在學校學過什麼，不會教太難，也不會重複教
- 📝 大綱一版一版改（v0.1、v0.2…），每一版都列出「需要你決定的事」，不會一次丟一大包給你
- 🚨 你的想法可能讓課上不完、太難或超出範圍時，會當下提醒你，並給你幾個保留原本想法的辦法
- 📖 不懂的名詞隨時問，附名詞小辭典

**最後交給你 What you get at the end**
- 📄 **教案（中文版＋英文版）**：基本資料卡、學習目標、核心單字、每一頁的步驟和**中英對照的老師引導句**、學生可能的反應、可能被問到的問題、時間不夠時的備案、物品清單
- 🖼️ **簡報規劃**：每一頁要放的文字、畫面說明，以及可以直接貼到 AI 繪圖或簡報工具的 prompt
- ✏️ **學習單**：學生版和答案版
- 🎲 **課堂活動與遊戲**：玩法、分組、需要的道具，也可以做成 Kahoot
- 🏃 **大地遊戲**：關卡、題庫、跑關流程
- ✅ **交付前的品質檢查**：時間夠不夠、難度合不合適、教案和簡報、學習單的內容有沒有一致
- 📦 輸出 Word（.docx）和 PDF

**While you design**
- 🧭 Clarifies your needs first — time, students, room, equipment — explaining why each question matters, with defaults if you're not sure
- 🗺️ Planning a series? Maps out each lesson's topic and difficulty so they build on each other
- 🔍 Checks what students have already learned at school, so the lesson is neither too hard nor repetitive
- 📝 Outlines in versions (v0.1, v0.2…), each ending with the decisions that are yours to make
- 🚨 Flags it right away when an idea would make the lesson overrun, too hard or out of scope — with ways to keep your idea
- 📖 Ask about any term anytime; a glossary is included

**At the end**
- 📄 **Lesson plan (English + Chinese)**: info card, objectives, key vocabulary, step-by-step guidance with **bilingual teacher scripts**, expected student responses, likely questions, a backup plan if time runs short, materials list
- 🖼️ **Slide plan**: text and visuals for every slide, plus prompts ready to paste into AI image or slide tools
- ✏️ **Worksheets**: student and answer versions
- 🎲 **Classroom activities and games**: rules, grouping, props — Kahoot-ready if you like
- 🏃 **Ground games**: stations, question bank, running order
- ✅ **A quality check before delivery**: timing, difficulty, and whether the lesson plan, slides and worksheets all match
- 📦 Output as Word (.docx) and PDF

## 安裝 Install

這套 skill 是一般的文字檔（Markdown），可以用在大部分支援自訂指示和上傳檔案的 AI。先下載這個 repo（Code → Download ZIP），再依你用的 AI 選一種方式：

This skill is plain text (Markdown), so it works with most AI assistants that support custom instructions and file uploads. Download this repo (Code → Download ZIP), then pick the option for your AI:

### 任何 AI：專案／自訂指示 Any AI: project or custom instructions
適用 ChatGPT（Project 或自訂 GPT）、Gemini（Gem）、Claude（Project）等。 Works with ChatGPT (Projects or custom GPTs), Gemini (Gems), Claude (Projects) and others.
1. 建立一個新的專案、GPT 或 Gem
2. 把 `skills/lesson-plan-design/` 裡的檔案上傳到知識庫
3. 把 [`project-instructions.md`](project-instructions.md) 的內容貼到指示欄位

### 支援 Skills 的 AI（例如 Claude）AIs that support skills (e.g. Claude)
1. 把 `skills/lesson-plan-design` 資料夾單獨壓縮成 `lesson-plan-design.zip`
2. 在 AI 的設定中找到 Skills，上傳這個 zip

### Claude Code
```bash
git clone https://github.com/chanelhwung94-glitch/lesson-plan-design.git
cp -r lesson-plan-design/skills/lesson-plan-design ~/.claude/skills/
```

## 使用方式 Usage

裝好之後，直接跟你的 AI 說你想做的課：

> 我想設計一堂給 4–6 年級的雙語課，主題是動物的家，60 分鐘。

> 我想做一個 4 堂課的系列，教營隊的國中生認識環保，先幫我排系列大綱。

> I want to design a 40-minute lesson for beginners on world festivals.

## 關於我 About me

大家好，我是 Chanel，台灣青年教育組織 Youth Impact Taiwan 的創辦人。我並非教育本科出身，過去三、四年透過 Youth Impact Taiwan 的志工服務，投入教案設計，並走訪多所偏鄉國小帶領課程。為了讓教學更有依據，我也進修了 TESOL（英語作為外語教學）課程。這套 skill 整理了我在實務與進修中累積的設計方法，希望幫助同樣想投入教學、卻不知從何開始的人。教學之路沒有標準答案，相信還有許多更資深、更優秀的老師，非常歡迎不吝指教，一起讓這套方法更完善。

Hi, I'm Chanel, founder of Youth Impact Taiwan, a youth education organisation in Taiwan. I don't come from an education background. Over the past three to four years, through volunteer work with Youth Impact Taiwan, I have designed lesson plans and taught in many rural elementary schools across Taiwan. To ground this work in theory, I also undertook TESOL (Teaching English to Speakers of Other Languages) training. This skill brings together the design approach I have developed through practice and study, for anyone who wants to teach but isn't sure where to begin. There is no single right way to teach, and many experienced educators will know far more than I do — your feedback and suggestions are warmly welcome.

## 授權 License

[CC BY 4.0](LICENSE) — 歡迎使用、修改、分享，請標註 Youth Impact Taiwan。字型、字表、課本等第三方資料不在此授權範圍內。

歡迎開 issue 或 pull request 分享你的改良。 Issues and pull requests welcome.

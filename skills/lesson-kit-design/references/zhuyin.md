# Zhuyin · 注音

Whenever the class includes any grade 1–3 students, they need zhuyin on every Chinese character in student-facing material: worksheets, slides, game cards. This is a required condition of the kit (see `lesson-plan.md`). Teacher-only material (the lesson plan itself, answer keys) doesn't need it.

This is the **default for Taiwanese elementary schools**. If your learners aren't young Taiwanese readers, skip this file and ask what reading support fits them instead (e.g. pinyin, furigana, picture cues, or none).

## Quick start for beginners 新手三步驟
1. **下載字型：** 到翻轉教育的注音字型文章（連結見下方），下載「楷體注音（字嗨注音標楷）」，解壓縮後點兩下字型檔、按「安裝」，重開 Word／PowerPoint。
2. **設定破音字：** 把學生要看的中文貼到「讀音選擇工具」，檢查破音字的讀音，再貼回文件。
3. **確認：** 在 Word 選取中文、換成字嗨注音標楷，看到每個字右邊都有注音就成功了；匯出 PDF 後再看一次。

If an AI is generating the document, send it the installed font file (or tell it the font is installed on the computer that will open the file), so the PDF uses the right font.

## Recommended method: a Bopomofo IVS zhuyin font
Use a zhuyin font that follows the **注音IVS字型規格 (Bopomofo IVS font specification)** — https://github.com/ButTaiwan/bpmfvs. A zhuyin font draws each character with its bopomofo already attached on the right side, in the standard vertical layout, so you only apply the font to the Chinese text — no manual typing of symbols, no ruby fields.

- **Download:** from the project's Releases page. Fonts aren't bundled with this skill; each user downloads and installs them (see the project's licence notes). A Chinese guide with download links for each font: 翻轉教育〈注音字體下載：精選7款最好用的免費注音字型〉https://flipedu.parenting.com.tw/article/009835
- **Supported:** Windows 7+, macOS 10.6+, Microsoft Office 2010+, Adobe InDesign / Illustrator CS4+; also usable in PowerPoint and Canva.

### Which font for what
| Use | Font | Notes |
|---|---|---|
| **All Chinese body text (default)** | 楷體注音 — **字嗨注音標楷** | Kaishu meeting MOE standards; satisfies the 標楷體 rule |
| Character-writing practice (fill in the character) | **字嗨注音加框** | An empty box ▢ with zhuyin beside it — kids write the character in the box |
| Titles or emphasis only, if the designer chooses | 芫荽注音 (hand-written Kaishu), 源流／源雲／源樣注音明體, 字嗨注音宋體, 源石注音黑體, 源泉注音圓體 | Never for body text — body text stays in 楷體注音 |

### Using the fonts in Canva
Upload the installed font file to Canva as a brand font (Canva home → 品牌 Brand → 品牌字型 Brand fonts → 上傳字型 Upload font), then pick it from the font list. Font upload may depend on the Canva plan; if upload isn't available, tell the designer.

## Polyphonic characters 破音字
A character with several readings (的、了、著、會、長、行、重、樂、看、不、一…) shows its default reading unless told otherwise. In this spec, an alternate reading is chosen by placing an **ideographic variation selector (IVS)** right after the character — for example 會 + U+E01E1 shows its second reading ㄎㄨㄞˋ. Because the selector is part of the text, the chosen reading survives copy-and-paste between programs.

How to set readings:
1. **Preferred:** paste the student-facing Chinese text into the project's **讀音選擇工具 (reading selection tool)** — it detects readings from context automatically — check and adjust the reading for each polyphonic character in context, then copy the result into the document. See the `guide` folder of the project.
2. **When generating documents in code:** keep the IVS characters in the text exactly as produced by the tool. Only insert a selector yourself when you're sure of the correct one from the spec's data for that character; otherwise leave it and list the character for the designer to check.
3. Older Adobe workflows may use stylistic sets (文體集) instead; those choices can be lost on copy-and-paste, so prefer IVS.

Always list the polyphonic characters you found and the reading you chose, so the designer can check them.

## In the document
1. Install the font where the document is generated and on every computer that will open the .docx.
2. Set 字嗨注音標楷 as the **East Asian font** for Chinese text on student-facing pages; keep Times New Roman for English.
3. Use 16pt+ for Chinese on Basic worksheets — the bopomofo is drawn at a fraction of the character size.
4. Export to PDF with fonts embedded (`pdffonts file.pdf` should list the zhuyin font) and check the readings visually.

## Before sending
- [ ] Every Chinese character on student-facing pages shows zhuyin, on the right, vertical
- [ ] Polyphonic characters set in context (IVS) and listed for the designer
- [ ] PDF has the zhuyin font embedded
- [ ] Printed test page is readable at the chosen size

## If the font isn't available
Tell the designer and ask them to install it. Word's Phonetic Guide (注音標示) or typing bopomofo by hand works for a few words only — say so if you fall back to it.

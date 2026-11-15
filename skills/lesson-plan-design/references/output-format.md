# Output Formats · 輸出格式

## Language versions
The **lesson plan** is delivered in **English (required) and Chinese**, with identical structure and file format, named the same apart from a language suffix, e.g. `…_教案_EN.docx` / `…_教案_ZH.docx`. Other documents (worksheets, activity write-ups, series map) are single files; worksheets and slides are bilingual on the page.

## Lesson plan, worksheet, activity write-up → .docx + .pdf
Deliver each document in two formats, same name, same folder:
- **.docx** — the editable source, for the next designer to revise
- **.pdf** — for printing and sending to volunteers and schools

Build the .docx with whatever docx tooling is available (if a docx skill is listed, load it first). Then convert to PDF (e.g. LibreOffice `soffice --headless --convert-to pdf`) and **open the PDF to check it**: fonts embedded, zhuyin rendering correctly, nothing overflowing the page, answer key on its own page.

Font setup in the .docx (see `lesson-plan.md` for why):
- East Asian font: 標楷體 (Windows: `DFKai-SB`; macOS: `BiauKai`; or the zhuyin font for student-facing material whenever the class includes grade 1–3 students — see `zhuyin.md`)
- Latin font: Times New Roman
- Set both on each run (`w:eastAsia` and `w:ascii`/`w:hAnsi`), so mixed Chinese–English lines use the right font for each script.

If the font isn't installed where the file is generated, the PDF will silently fall back to another font. Check the PDF's fonts (e.g. `pdffonts file.pdf`); if 標楷體 or the zhuyin font is missing, tell the user and ask for the font file rather than shipping a PDF in the wrong font.

Also offer the lesson plan as Markdown when the user keeps plans in Google Docs or Notion — they can paste it in.

## Slides → follow the user's own template
Teams build slides in different tools (Canva, Google Slides, PowerPoint, Gamma, AI image tools). Don't impose one.

1. At intake, ask: "Which tool do you make slides in, and can you share a template or a previous deck you like?"
2. **If they share a template or past deck** (.pptx, PDF export, screenshots, or a link): study it — layout per slide type, fonts, colours, where the title/picture/footer sit, how the bilingual text is arranged — and make the new deck mimic it. With a .pptx, build from it directly (if a pptx skill is listed, load it first). Otherwise, put a short "template description" at the top of the slide skeleton and write every per-slide prompt to match it.
3. **If they have no template:** deliver the slide skeleton with per-slide prompts (`templates/slide-skeleton.md`) and a neutral, child-friendly style line. Don't invent branding.

Either way, the slide skeleton stays the source of truth: slide number ↔ lesson-plan page numbers must match.

## Kahoot → .md + .csv
See `practice-design.md`.

## File naming
Follow the house style. Default example: `{code}_{topic}_{level}_{type}[_注音版].{ext}`.

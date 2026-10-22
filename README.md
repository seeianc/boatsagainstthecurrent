# Boats Against the Current

A top-down adventure game through F. Scott Fitzgerald's *The Great Gatsby* (1925, public domain in the US), for 11th-grade English. Students play Nick Carraway and complete the novel's nine chapters in order.

Everything runs in one `index.html` file. There is no build step, no server and no AI. Progress saves in the browser, so students can stop and pick up again next class.

## Play it

- **Locally:** open `index.html` in a browser.
- **On GitHub Pages:** upload `index.html` and this README to the root of a public repository. Go to **Settings → Pages**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.

## The world

Six screens, explored the classic way by walking off the edge of one screen into the next:

| | | |
|---|---|---|
| East Egg (the Buchanans) | Courtesy Bay (the green light) | West Egg (Gatsby's mansion, Nick's cottage) |
| New York (Myrtle's apartment, the Plaza, Wolfsheim) | The Valley of Ashes (Wilson's garage, Eckleburg) | The Motor Road |

New York and the valley open in Chapter II. A gold **!** marks the next task, and the minimap blinks where to go.

## How it teaches the standards

**Cite strong textual evidence, explicit and implicit, including inconsistency and ambiguity.**
- Talking and looking adds 41 quotations to Nick's evidence, each tagged by speaker and chapter.
- Inference checks ask what a line *implies*, for example Daisy's "beautiful little fool" or Gatsby's "Her voice is full of money."
- At Gatsby's parties, **rumors** attack, and Nick's pen pops them. Getting hit costs *credibility*.
- The **Case File** collects six claims: Catherine's Catholic story, the murder and spy rumors, Nick's own claim to honesty, Gatsby's wealthy Midwestern parents, Oxford, and who drove the death car. Students give a verdict (supported, contradicted, partly true, ambiguous) and pin the quotes that prove it. Some claims can't be settled until later chapters supply the evidence, so students learn to revise.

**Provide accurate summaries that show relationships among key details.**
- Each chapter ends at Nick's **writing desk**. Students choose the four key events, in order, from six cards that include two decoys.
- They then choose the sentence that best explains how the events connect.
- The game saves the summary to the journal.

**Determine themes and analyze their development, including how elements interact.**
- Six motifs (the green light, Eckleburg's eyes, the valley of ashes, cars, clocks and time, weather) are logged to a **motif timeline** each time they return, with what they mean at that point.
- At Chapters III, V and VII, a theme check asks how several elements build on each other.
- After Chapter IX, students build a **final argument**: they choose one of four themes and three moments from at least three chapters that develop it. The game checks the choices and assembles a paragraph.

## Controls

| Action | Keyboard | Touch |
|---|---|---|
| Walk | Arrows or WASD | D-pad |
| Talk, look, continue | E or Enter | A |
| Swing pen | Space | B |
| Answer | 1–3 | Tap |
| Journal | J | Journal button |

## For teachers

- **Start at a later chapter** (from the Menu) fills in earlier chapters automatically, for classes already partway through the book.
- **Copy my journal** exports the case file, summaries, motif timeline and final argument as text for students to hand in.
- All content lives in `EVID`, `CLAIMS`, `MOTIFS`, `THEMES` and `CH` near the top of the script, in plain JavaScript. Each chapter's `beats` are the tasks in order. Each beat has dialogue `lines`, `ev` (quotes it awards), an optional `ask` (an inference question), an optional `motif` entry and an optional `claim`.

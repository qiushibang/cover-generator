---
name: cover-generator
description: This skill should be used when creating or revising a 3:4 Chinese social-media cover from a user's personal photo and either manual copy, an uploaded document, or the current work directory. It first presents six bundled reference templates for selection, then creates a diagonally dynamic, non-boxy Chinese cover that faithfully follows the selected template.
---

# Cover Generator

Create a finished 3:4 Chinese social-media cover from one bundled template, the user's personal portrait, and a content source. Keep the selected template's distinctive visual system while applying the mandatory shared diagonal-motion treatment defined below.

## Start With the Template Gallery

Show the complete six-template gallery before asking the user to choose a template. Open and render all six images in `assets/templates/` inline in one response; place the template number and a short use case next to each image.

The bundled gallery assets are synthetic, faceless illustrations. Keep the installed template gallery free of real-person photography, identifiable faces, third-party logos, and watermarks. A real person may appear only in a newly generated final cover when the user has supplied that portrait for the task.

| Template | File | Use for |
| --- | --- | --- |
| 01 | `01-classroom-checklist.png` | tutoring, courses, learning plans, and structured benefits |
| 02 | `02-dark-high-contrast.png` | punchy short-video formulas, copywriting, and operational how-tos |
| 03 | `03-light-tech-code-card.png` | developer workflows, coding, tools, and technical experiments |
| 04 | `04-light-tech-product-card.png` | product workflows, integrations, and multimodal/tool introductions |
| 05 | `05-notebook-callouts.png` | evaluations, product methods, and annotated explainers |
| 06 | `06-neon-self-media-board.png` | creator tools, skills, workflows, and feature checklists |

Ask the user to select one number. When no selection is given, recommend one template from the content source, but do not generate until the user confirms the number. Never blend two templates.

## Collect the Portrait and Content Source

Obtain one clear, well-lit personal photo with the upper body visible. Preserve that person's recognizable face, hairstyle, clothing, and natural pose. Never use a person visible in a template as the output person.

Accept exactly one of these content sources. Do not force the user to handwrite cover copy when a usable source is supplied.

1. **Manual copy**: use the user-provided title, subtitle, and points.
2. **Uploaded document**: read the attached document, identify its title, core topic, target audience, verified benefits, and up to three concrete points. Draft the cover copy automatically.
3. **Current work directory**: inspect only project-level public context first: `README*`, top-level documentation, `docs/`, package/project manifests, and user-named files. Exclude `.env`, credentials, private keys, lockfiles, dependency directories, build outputs, caches, and data folders unless the user explicitly names one. Draft the cover copy only from supported facts found in those files.

Open `references/content-source-workflow.md` before extracting document or directory content. For a document, use the appropriate document-reading capability. For a directory, begin with a bounded file listing and read the smallest set of relevant files; do not scan unrelated personal or secret material.

Generate the cover copy directly from the source: a topic pill, one two-line headline, one short subtitle or evidence line, and two or three card labels. Use concise Chinese that remains legible at thumbnail size. Do not fabricate outcomes, metrics, customers, compatibility, or product features. When the source lacks a supported claim, use an accurate general framing rather than inventing one.

## Apply Mandatory Diagonal Motion

Treat every cover as vertically framed but diagonally composed. Apply these requirements to every template:

- Keep the canvas 3:4 vertical, but place the dominant background field, light band, board, screen, or color block on a 6–12 degree diagonal axis. Do not use a flat, centered, horizontal background.
- Rotate or shear the headline group 4–9 degrees while keeping it fully readable. Use expressive oblique display lettering or a slightly handwritten/italic Chinese title treatment; avoid rigid upright square sans-serif title blocks.
- Put the title's highlight strip, supporting card, and prominent decorative rule on related but not identical diagonal axes. Make the composition feel intentionally layered rather than as if the entire canvas was simply rotated.
- Keep internal detail labels easy to read. Let them inherit the angle of their card or panel rather than forcing every small line into a perfectly horizontal square grid.
- Preserve the selected template's recognizable palette, density, card geometry, presenter position, and decorative motifs. The diagonal-motion treatment is a shared overlay, not permission to borrow another template's visual language.

Read `references/template-guide.md` and inspect the selected template before writing the image prompt.

## Build the Image

1. Inspect the selected template, the supplied portrait, and the content source before generation.
2. Create the copy automatically from the selected source. Use every visible line verbatim in the generation prompt. When manual copy is too long, offer a shortened version before generation; when document/directory content is too long, condense it without changing facts.
3. Use the built-in image-generation tool. Supply the selected template as the layout/style reference and the supplied portrait as the identity reference. Generate a new cover rather than editing the template asset.
4. State every selected-template invariant and every mandatory diagonal-motion requirement in the prompt: 3:4 canvas, slanted background, oblique non-boxy headline, diagonal card axes, text placement, portrait scale/position, palette, and decorations.
5. State that the only replaceable elements are the source-derived text, permitted generic icons, and the supplied person. Treat the faceless template figure as a position and scale guide only. Preserve no source-template wording, creator identity, logo, or watermark.
6. Inspect the result at full size and thumbnail size. Regenerate with one focused correction when template fidelity, diagonal composition, Chinese legibility, portrait likeness, or factual accuracy fails.

## Revision Rules

For a revision, change only the requested copy, portrait detail, or content-source interpretation. Preserve the chosen template, diagonal background axis, headline tilt, non-boxy display treatment, palette, card anchors, and presenter placement unless the user explicitly requests a different template or angle.

## Validate Before Delivery

Confirm all of the following:

- Display all six templates before template selection.
- Use exactly one template and retain its distinctive visual system.
- Use an intentional diagonal background and a readable oblique, non-boxy headline; do not merely rotate the whole canvas.
- Use source-derived copy only, with no fabricated claims.
- Use only the user-supplied person and retain a natural, recognizable likeness.
- Render requested Chinese accurately and legibly at thumbnail size.
- Include no copied template wording, creator identity, logo, watermark, or unrelated brand mark.

Report the selected template number, content source, and generated file path when delivering the result.

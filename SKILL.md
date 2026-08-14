---
name: smkt-photo-ink
description: Transform a user-supplied photo into a fixed source-colour ink-and-wash editorial illustration. Use when a user asks to stylize a photo. Do not use for article visuals, diagrams, text-led posters, or unrelated image generation. Trigger phrases: "照片水墨风格化", "把照片画成水彩", "照片做成水墨插画".
---

# Photo Ink Editorial

Turn the uploaded photograph into one coherent, full-scene editorial illustration. Treat every visible element—people, animals, objects, and background—with the same style.

## Fixed treatment

- Deliver every result on a vertical 3:5 canvas. When the source ratio differs, recompose the illustration to fit it: retain all main subjects, their poses, relative scale, key scene anchors, and major left/right/top/bottom relationships; add quiet paper or setting breathing room as needed, and crop only non-defining empty margins. Never crop, delete, duplicate, or replace a main subject to force the frame.
- Keep the main people, animals, or objects recognisable through their silhouette, defining features, clothing, markings, and visible colours. This is a hand-drawn interpretation, not pixel-identical preservation.
- Preserve the source photo’s colour families and their relationships as muted, translucent washes. Do not substitute a brand palette or add a brand-colour accent.
- Use a warm off-white, lightly textured paper ground; restrained near-black irregular ink contours; quiet watercolour/ink washes; and open, breathing light areas.
- Keep the scene readable at a glance. Preserve major zones and distinctive anchors, while grouping repeated foliage, flowers, tiles, railings, crowd details, pavement marks, or fabric creases into simple masses and a few selective lines.
- Render the whole image in the same language. Never leave a photographic cutout, realistic face, or photorealistic clothing over an illustrated background.
- Make the result clean and contemporary: no dense hatching, engraving, comic inking, polished vector-ad finish, typography, labels, borders, logos, signatures, or watermarks.

## Success criteria

The delivered image is a complete, recognisable ink-and-wash interpretation with no photographic elements left behind.

## Workflow

1. Inspect the actual uploaded image. Identify its main subject(s), defining features, major colour families, composition, and background anchors.
2. Use the image as an edit target with `image_gen`. For a local file, pass it through `referenced_image_paths`; for a chat attachment, include the smallest sufficient recent-image count. Never supply both.
3. Generate and directly deliver one full-scene edit using the fixed treatment. State the observed source-specific anchors in the prompt and explicitly require every visible subject to be redrawn in the same ink-and-wash language as the setting.

## Fixed prompt core

Use this core after the source-specific scene map:

> Transform the supplied photo into one coherent, complete hand-drawn editorial illustration on a vertical 3:5 canvas. Recompose only to fit that canvas: preserve all main subjects, their poses, relative scale, key scene anchors, major spatial relationships, and source-derived colour families; add quiet paper or setting breathing room as needed, and crop only non-defining empty margins. Never crop, delete, duplicate, or replace a main subject to force the frame. Render every person, animal, object, and background element in the same clean ink-and-wash language: warm off-white lightly textured paper, muted translucent source-colour washes, and a few restrained irregular near-black contours. Keep the main subjects recognisable but deliberately simplified; do not leave any photographic cutout, photorealistic face, or realistic clothing. Preserve major scene anchors, but group repeated detail into quiet shapes and selective lines with generous breathing room.

## Error handling and minimal change

- If no usable photo is attached, ask for one; do not invent the source scene.
- If generation fails, report the failure instead of inventing an output.
- Do not alter the source photo or fixed treatment to recover from a failure. Only request a usable replacement photo when needed; never auto-retry, switch tools, or create extra variants.
- If a user asks for a different visual style, a separate treatment, or an untouched photographic subject, explain that this fixed template only produces the established full-scene ink-and-wash treatment; do not add switches back into this Skill.

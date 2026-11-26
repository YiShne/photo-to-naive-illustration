# Prompt recipes

Use these as scene-specific scaffolds, not literal descriptions for every photo. Replace all braces before generation. Prompts are in English for portable reuse; communicate with users in their language.

## General template

```text
Use case: style-transfer.
Primary request: transform the content photo into one finished naive hand-drawn flat-color illustration.
Inputs: {photo input} is the content/edit target. {style inputs, if actually attached} are visual style references ONLY; do not import their objects, people, letters or signatures.
Essential subject: {main subject, count, defining silhouette or identity cues}.
Essential relationship: {pose, interaction, arrangement or visual joke that must remain}.
Composition: {aspect ratio, subject placement, useful scale adjustment and negative space}.
Simplification: {specific items to remove or condense; specific props to retain}.
Visual language: bold black slightly wobbly hand-drawn rounded outlines, organic asymmetry, simple readable shapes, few interior strokes, playful minimal picture-book composition. Clean flat opaque solid color blocks.
Palette: {small set of source-appropriate colors}; use a uniform {background color} backdrop.
Constraints: preserve {core invariants}. No photographic texture, gradients, shading, gloss, refraction or 3D volume. No added objects, characters, faces, text, signatures or watermarks unless explicitly requested.
```

Avoid forcing fixed subject sizes or numbers of simplified marks across all photos. The examples below record successful treatments; adapt their reasoning.

## Still life: iced water on blue cloth

Retain one tapered drinking glass, a long bent drinking straw leaning upper right, a few chunky ice shapes and a broad diagonal blue napkin. Enlarge the glass as the focus. Merge table and background into warm cream. Represent the glass with pale blue flat fill and a black silhouette, ice with irregular white rounded blocks, and the straw with a narrow pale gray shape. Remove reflections, refraction, glass fluting, cloth weave and folds. Do not give the glass a face. See `iced-glass.png`.

## Outdoor object: flower balloon over a red roof

Retain one flower-shaped balloon, white scalloped petals, a yellow center with the existing dot eyes and curved smile, a small knot and one trailing string. Enlarge it against a broad uniform blue sky. Reduce the buildings to a cropped cream house with a red sloped roof and a few loose tile marks. Remove power lines, towers and tiny distant detail. Keep the balloon recognizable as a balloon rather than turning it into a rooted plant. See `flower-balloon.png`.

## Playful food: fried egg on a clothesline

Retain exactly one fried egg held by exactly two upright tan wooden clothespins on one crossing line. Egg white hangs below the line; clothespins overlap its upper edge. Keep the single yellow yolk offset to one side. Use an asymmetrical lobed white silhouette and a yellow irregular circle with black contours. Reduce pegs to tan shapes with one short mechanism mark. Remove browned crust detail, bubbles, wood grain and shadows. Preserve generous blue negative space and do not add a face. See `hanging-egg.png`.

## People: applying the same grammar to a new photo

Preserve the actual main-person count, key pose/interaction, recognizable hairstyle, main clothing colors and important props. Use large round heads, short bodies, dot eyes, tiny mouths, mitten hands and bean shoes. Reduce clothing to broad color masses. Translate a hug through overlapping body silhouettes and hand placement, rather than realistic fingers or facial rendering. Remove background passersby if they are incidental; keep them if they are part of the user's intended subject. No bundled portrait example is supplied: derive this treatment from the written style rules and the user's photo.

## Focused revision phrases

- Flatten fills: “Keep the composition and contours unchanged. Replace all gradients, texture and shading with uniform solid fills in the existing palette.”
- Simplify: “Keep the main subjects and interaction. Remove {named secondary details}; reduce {object} to {named simple shapes}.”
- Stronger focus: “Keep the content and style. Enlarge {main subject} relative to {secondary elements}, retaining breathing room and the essential relationship.”
- Preserve identity cues: “Keep the simplified face language. Restore {hairstyle, glasses, distinctive garment or prop} from the source photo without adding realistic facial detail.”

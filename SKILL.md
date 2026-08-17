---
name: laosan-niulai-vision
description: Transform a supplied image into an original rough, abstract, low-poly rural-surreal visual built from oversized angular planes and primitive sculptural forms while preserving essential subject identity and composition. Use for stylizing portraits, animals, objects, or scenes; do not use for polished 3D rendering, exact restoration, faithful brand reproduction, or claims of official film affiliation.
---

# LaoSan NiuLai Vision

Turn a reference image into a rough, abstract geometric interpretation with a rural-surreal atmosphere. Favor primitive sculptural mass, blunt polygon cuts, visible irregularity, and handmade incompleteness over polished low-poly rendering.

## Workflow

1. Inspect the source before editing. Identify the subject, silhouette, pose, camera angle, composition, lighting direction, important colors, and identity-defining details.
2. Separate invariants from stylization freedom:
   - Preserve the subject count, placement, pose, key proportions, recognizable facial or object features, and any explicit user constraints.
   - Simplify secondary texture, background detail, and material transitions into deliberate polygonal planes.
3. Choose a transformation strength:
   - `light`: preserve recognition while replacing smooth surfaces with broad, uneven planes.
   - `rough`: oversized facets, blunt proportions, primitive sculptural mass, and visibly coarse material. Use this by default.
   - `extreme`: severe geometric reduction and stronger surreal distortion; keep only the core silhouette, subject count, pose, and key identity anchors.
4. Build the image prompt from the source analysis and the selected strength. Read [references/style-system.md](references/style-system.md) for visual decisions and failure corrections.
5. Generate or edit the image with the available image tool. For edits, pass the actual source image rather than describing it from memory.
6. Review the output against the preservation checklist. If a retry is needed, correct the specific failure instead of increasing every style attribute.

## Preservation Checklist

- Same number and type of primary subjects
- Recognizable silhouette, pose, expression, and identity cues
- Composition and crop remain close unless the user requested a change
- Important costume, fur, product, or prop colors remain traceable
- No invented text, logos, limbs, accessories, or background subjects
- Requested size, aspect ratio, and transparency are honored

## Prompt Construction

Describe what must remain before describing the style. Require oversized faceted planes, hard angular breaks, crude asymmetry, primitive carved mass, sparse facial detail, coarse matte surfaces, restrained earth colors, and flat or hazy cinematic light. Explicitly reject smooth skin, fine topology, glossy materials, cute stylization, polished 3D, photorealism, and commercial animation rendering. Avoid relying on a film title or another creator's name as the only style instruction.

Do not promise pixel-perfect preservation from a generative edit. When exact product graphics, typography, or logos must remain unchanged, state that a compositing or manual retouching workflow may be required.

## Boundaries

- Produce original visual interpretation; do not copy another repository's prompt text or present the work as an official film asset.
- Do not remove watermarks or ownership marks.
- Do not identify a real person from an image.
- Keep user-provided constraints above the default style system.

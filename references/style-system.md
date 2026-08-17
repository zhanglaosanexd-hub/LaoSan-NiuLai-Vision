# Visual Style System

Use this reference when composing the image prompt or diagnosing an unsatisfactory result.

## Core Visual Language

### Geometry

- Reduce forms into broad, readable polygonal planes.
- Keep large planes coherent; avoid noisy micro-faceting.
- Preserve the outer contour and identity-defining landmarks.
- Let facial features remain sparse and structural rather than smooth or hyper-detailed.

### Material

- Favor matte clay, weathered plaster, dry wood, coarse cloth, dusty fur, and muted stone-like surfaces.
- Keep highlights broad and soft. Avoid glossy plastic unless the source object requires it.
- Retain a small amount of tactile irregularity without adding random cracks or dirt.

### Color

- Start from the source palette, then compress it toward warm soil, faded straw, charcoal, muted green, fog blue, or oxidized red.
- Use one controlled accent color when the source contains a strong identifying hue.
- Keep shadows colored and cinematic rather than pure black.

### Light and Atmosphere

- Prefer low-angle directional light, soft overcast light, mist, dust, or restrained volumetric rays.
- Separate the subject from the background with value contrast or a thin rim light.
- Preserve readable facial planes and avoid crushing the image into darkness.

### Composition

- Maintain the source camera angle, crop, subject placement, and visual hierarchy by default.
- Simplify the background into a few large masses with depth layers.
- Use negative space deliberately; do not fill empty areas with invented props.

## Strength Profiles

### Light

Subtle planar simplification, source-faithful colors, gentle cinematic grading, minimal background abstraction.

### Balanced

Clear low-poly planes, compressed earthy palette, matte materials, atmospheric depth, preserved recognition and composition.

### Bold

Large geometric reductions, stronger silhouette emphasis, sparse surreal environment, dramatic but readable lighting. Preserve subject identity and count.

## Reusable Prompt Frame

Adapt this frame to the actual image instead of copying it verbatim:

> Edit the supplied image. Preserve [subjects, count, pose, silhouette, identity cues, composition, crop, key colors]. Reinterpret surfaces as [strength] low-poly cinematic forms using broad faceted planes and simplified geometry. Use [palette], [materials], and [lighting]. Simplify the background into [large depth layers]. Keep the image recognizable and restrained. Do not add [likely unwanted elements]. Output [aspect ratio, dimensions, transparency].

## Failure Corrections

| Failure | Targeted correction |
| --- | --- |
| Subject no longer resembles the source | Reduce abstraction on the face or key landmarks; restate identity cues and silhouette first |
| Image is too dark | Lift midtones, soften contrast, retain warm fill light, keep facial planes readable |
| Surface is too rough | Remove micro-texture and cracks; use larger matte planes with smoother value transitions |
| Looks like generic 3D | Add restrained asymmetry, rural material cues, haze, and cinematic color compression |
| Too many polygons | Replace micro-facets with broad planes and a cleaner silhouette |
| Background overwhelms subject | Reduce background detail, lower contrast, and restore subject-background value separation |
| Extra objects appear | Explicitly preserve subject count and prohibit invented props or figures |
| Product details drift | Reduce transformation strength around logos, proportions, edges, and functional parts |

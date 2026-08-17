# Visual Style System

Use this reference when composing the image prompt or diagnosing an unsatisfactory result.

## Core Visual Language

### Geometry

- Reduce forms into a small number of oversized, blunt polygonal masses.
- Use visibly uneven plane sizes, hard breaks, crude asymmetry, and occasional awkward proportions.
- Prefer primitive carving and folded-paper mass over clean mesh topology.
- Keep the geometry intentionally coarse; avoid decorative micro-faceting and tidy subdivision.
- Preserve the outer contour and identity-defining landmarks.
- Let facial features become sparse structural marks: wedge-like nose, recessed eye planes, blocky cheek and jaw masses.

### Material

- Favor raw clay, chipped plaster, dry mud, roughly cut wood, coarse cloth, dusty fur, and unfinished stone-like surfaces.
- Allow uneven color fields, blunt edges, and restrained surface abrasion.
- Keep highlights sparse and dull. Avoid polished plastic, clean bevels, smooth skin, subsurface scattering, or studio-perfect materials unless the source object absolutely requires them.

### Color

- Start from the source palette, then compress it toward warm soil, faded straw, charcoal, muted green, fog blue, or oxidized red.
- Use one controlled accent color when the source contains a strong identifying hue.
- Keep shadows colored and cinematic rather than pure black.

### Light and Atmosphere

- Prefer flat overcast light, hard low-angle light, dusty haze, or simple theatrical illumination.
- Separate the subject from the background with value contrast or a thin rim light.
- Preserve readable facial planes and avoid crushing the image into darkness.

### Composition

- Maintain the source camera angle, crop, subject placement, and visual hierarchy by default.
- Simplify the background into a few large masses with depth layers.
- Use negative space deliberately; do not fill empty areas with invented props.

## Strength Profiles

### Light

Subtle planar simplification, source-faithful colors, gentle cinematic grading, minimal background abstraction.

### Rough — Default

Oversized blunt planes, crude asymmetry, primitive sculptural anatomy, compressed earthy palette, raw matte materials, and restrained cinematic atmosphere. Recognition comes from silhouette and a few identity anchors rather than detailed modeling.

### Extreme

Severe geometric reduction, deliberately awkward massing, sparse surreal environment, and only essential identity anchors. Preserve subject count, pose, and core silhouette.

## Reusable Prompt Frame

Adapt this frame to the actual image instead of copying it verbatim:

> Edit the supplied image. Preserve [subjects, count, pose, core silhouette, essential identity anchors, composition, crop, key colors]. Rebuild it as [strength] rough geometric sculpture using a very small number of oversized angular planes, blunt edges, crude asymmetry, awkward primitive proportions, sparse facial marks, and raw matte material. Use [palette] and [simple lighting]. Simplify the background into [large depth layers]. It must feel abstract, coarse, handmade, and slightly unfinished—not like polished low-poly 3D. Avoid smooth skin, fine topology, glossy materials, clean bevels, photorealism, cute character rendering, and commercial animation aesthetics. Do not add [likely unwanted elements]. Output [aspect ratio, dimensions, transparency].

## Failure Corrections

| Failure | Targeted correction |
| --- | --- |
| Subject no longer resembles the source | Reduce abstraction on the face or key landmarks; restate identity cues and silhouette first |
| Image is too dark | Lift midtones, soften contrast, retain warm fill light, keep facial planes readable |
| Surface is too rough | Remove micro-texture and cracks; use larger matte planes with smoother value transitions |
| Looks too polished or beautiful | Remove clean bevels and smooth gradients; enlarge the planes, distort their spacing, dull the material, and introduce blunt asymmetry |
| Looks like generic 3D | Reduce mesh sophistication; use primitive carved masses, raw rural material cues, flat light, and compressed color |
| Too many polygons | Cut the plane count aggressively; merge facial and body surfaces into oversized blocks |
| Still not abstract enough | Preserve only silhouette, pose, subject count, and 3–5 identity anchors; rebuild everything else as crude geometric mass |
| Background overwhelms subject | Reduce background detail, lower contrast, and restore subject-background value separation |
| Extra objects appear | Explicitly preserve subject count and prohibit invented props or figures |
| Product details drift | Reduce transformation strength around logos, proportions, edges, and functional parts |

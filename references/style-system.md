# Visual Style System

This system describes an original rural low-budget CGI language. Apply it as rendering decisions, not as a named-film imitation.

## Layer Checklist

### 1. Model and Proportion

- Build the subject from simple early-CGI meshes with a low vertex count and broad rounded masses.
- Use crude Gouraud-like smooth shading across the mesh. Let the low vertex count show mainly in the silhouette, joints, and proportion—not as hundreds of differently colored facets.
- Prefer blunt cylinders, inflated torsos, wedge-like noses, mitten hands or paws, and visibly simplified joints.
- Allow naive asymmetry and slightly incorrect anatomy: large head, short limbs, thick neck, wide-set or uneven eyes.
- Keep the silhouette and 3–5 identity anchors readable.
- Avoid both extremes: no polished character topology and no hard-edged clay-block sculpture.

### 2. Face and Expression

- Treat eyes, lips, nostrils, brows, and markings as sparse applied features on a simple head volume.
- Use fixed or slightly misaligned gaze, limited eyelid deformation, stiff mouth shapes, and restrained expression.
- Preserve the source expression in simplified form; do not automatically make every subject cute, angry, or human-like.
- For animals, preserve species anatomy unless the source or user requests anthropomorphism.

### 3. Texture Mapping

- The main signature is coarse texture mapping, not surface damage.
- Use visibly low-resolution fur, skin, fabric, bark, grass, and rock maps with soft pixels and uneven scale.
- Allow mild stretching around cheeks, shoulders, joints, and curved forms; slight seam or registration imperfections are useful.
- Markings may look stamped, tiled, or painted onto the geometry.
- Keep surfaces mostly matte with simple color response.
- Avoid detailed procedural fur, micro-cracks, heavy plaster relief, glossy PBR materials, and realistic subsurface skin.

### 4. Color

- Preserve identifying source colors, then compress them into a small palette.
- Favor bold artificial color blocks: mustard yellow, oxidized orange-red, dark bottle green, muddy brown, charcoal, dull blue, and off-white.
- Permit strong subject/background separation and slightly dirty saturation.
- Avoid refined cinematic teal-orange grading or tasteful desaturation that makes the result look premium.

### 5. Light and Render

- Use flat ambient illumination with one broad directional source.
- Highlights should be blunt and simple; shadows should be shallow, soft, or weakly attached.
- Allow slightly inconsistent light between subject and background if the composite remains readable.
- Maintain visible midtones. Do not crush the face into darkness.
- Avoid beauty lighting, glossy rim lights, volumetric spectacle, ray-traced realism, and studio-perfect contact shadows.

### 6. Environment and Composition

- Preserve the source crop, camera height, subject placement, and visual hierarchy by default.
- Rebuild backgrounds as naive stage sets: flat ground, painted or gradient sky, repeated lollipop-like trees, simple rock walls, dark shrubs, and sparse props only when supported by the source.
- Use primitive repeated foliage and obvious texture reuse rather than detailed natural scenery.
- Favor frontal medium shots, centered confrontation, simple shot/reverse-shot staging, or source-faithful framing.
- Do not invent film-specific characters, scenery, captions, or narrative events.

### 7. Image Finish

- Finish as an older digital render or compressed game cutscene: modest resolution, soft edges, restrained aliasing, faint grain, and mild compression.
- Texture detail should soften before silhouette readability is lost.
- Black side mattes, subtitles, scanlines, or timestamp artifacts are optional only when explicitly requested; never add them by default.

## Strength Profiles

### Light

Mostly faithful proportions and color, with primitive modeling, mildly coarse maps, simplified background, and subtle digital softness.

### Scene — Default

Rounded low-poly anatomy, awkward rigging, fixed gaze, visible low-resolution texture maps, artificial color blocks, flat theatrical light, naive rural stage-set scenery, and restrained compressed-video finish.

### Uncanny

More distorted proportions, rigid expression, stronger texture stretching, reduced scenery, obvious model/lighting mismatch, and greater digital degradation. Preserve subject count, pose, silhouette, and identity anchors.

## Reusable Prompt Frame

> Edit the supplied image. Preserve [subject count, pose, silhouette, 3–5 identity anchors, crop, composition, key colors]. Rebuild it at [strength] as an uncanny rural low-budget CGI frame: primitive early-CGI mesh with a low vertex count, broad rounded silhouette and crude Gouraud-like shading; naive proportions; stiff rigging and gaze; sparse facial deformation; low-resolution texture maps stretched over simple geometry; flat ambient light; blunt highlights; weak contact shadows; simplified stage-set background; and restrained old-digital softness. Keep the result recognizable but structurally awkward and inexpensive-looking. Avoid visible micro-faceting, mosaic-like polygon shading, polished animation, clean topology, detailed fur, physically based materials, beauty lighting, photorealism, clay sculpture, stone carving, invented characters, text, logos, and props.

## Failure Corrections

| Failure | Targeted correction |
| --- | --- |
| Looks like a clay or plaster sculpture | Remove relief, cracks, and carved edges; restore smooth primitive volumes with flat low-resolution maps |
| Looks like polished low-poly art | Simplify the rig and lighting; lower texture resolution; weaken contact shadows; add mild map stretching and fixed gaze |
| Too faceted | Stop rendering individual polygons as colored tiles; use broad rounded silhouettes, crude Gouraud-like shading, and texture-driven detail |
| Too photoreal | Remove detailed fur/skin and PBR response; flatten light and reduce material complexity |
| Too cute or commercial | Reduce eye sparkle and facial animation; use stiff mouth shapes, neutral gaze, naive anatomy, and dirty saturation |
| Not uncanny enough | Introduce slight proportion error, gaze misalignment, texture-scale mismatch, and subject/background lighting mismatch |
| Subject no longer resembles source | Restore silhouette, pose, key markings, gaze, and 3–5 identity anchors; reduce distortion elsewhere |
| Background overwhelms subject | Reduce it to flat ground, simple sky, and a few repeated primitive masses |
| Too dark | Lift midtones and use flat ambient fill while keeping simple directional shading |
| Extra content appears | Restate exact subject count and prohibit invented characters, captions, props, and scenery |

---
name: laosan-niulai-vision
description: Transform a supplied image into an original uncanny rural low-budget CGI frame with primitive geometry, stretched low-resolution textures, stiff posing, flat theatrical lighting, and preserved subject identity and composition. Use for stylizing portraits, animals, objects, or scenes; do not use for polished 3D rendering, exact restoration, faithful brand reproduction, or claims of official film affiliation.
---

# LaoSan NiuLai Vision

Turn a reference image into an uncanny rural low-budget CGI frame. The defining roughness should come from crude modeling, awkward rigging, low-resolution texture mapping, flat lighting, and simple compositing—not from turning the subject into a clay or stone sculpture.

## Workflow

1. Inspect the source. Identify subject count, silhouette, pose, camera angle, crop, setting, dominant colors, and 3–5 identity anchors.
2. Lock invariants before stylizing: keep subject count, placement, pose, core silhouette, identity anchors, and explicit user constraints.
3. Choose a strength:
   - `light`: source-faithful composition with mild primitive modeling and texture degradation.
   - `scene`: obvious low-budget CGI, awkward anatomy, coarse texture maps, stiff staging, and flat theatrical light. Use this by default.
   - `uncanny`: stronger proportion distortion, rigid expression, simplified scenery, and degraded rendering while retaining the core silhouette and identity anchors.
4. Read [references/style-system.md](references/style-system.md) before building the prompt. Diagnose by layer instead of adding generic “roughness.”
5. Edit with the actual source image. Do not reconstruct the source from memory.
6. Review the result. Correct only the failing layer: model, texture, rig/pose, light, environment, or image finish.

## Preservation Checklist

- Same number and type of primary subjects
- Recognizable silhouette, pose, expression, and 3–5 identity anchors
- Composition and crop remain close unless the user requested a change
- Important fur, costume, product, or prop colors remain traceable
- No invented text, logos, limbs, accessories, or background subjects
- Requested aspect ratio, dimensions, and transparency are honored

## Prompt Construction

State preservation constraints first. Then describe the result across six layers:

1. primitive early-CGI mesh with a low vertex count and coarse smooth shading;
2. low-resolution stretched or slightly misregistered texture map;
3. stiff rigging, fixed gaze, and limited facial deformation;
4. flat ambient light with blunt highlights and weak contact shadows;
5. simplified rural stage-set environment made from repeated primitive forms;
6. soft low-resolution image finish with restrained grain, aliasing, and compression.

Use “uncanny,” “naive,” “stiff,” and “low-budget” as structural qualities. A low vertex count must not become a mosaic of visible micro-facets: prefer broad rounded silhouettes, crude Gouraud-like shading, and texture-driven detail. Explicitly reject polished animation, physically based materials, clean topology, beauty lighting, detailed fur, clay sculpture, and stone carving. Do not rely on a film title or creator name as the only style instruction.

Do not promise pixel-perfect preservation. Exact typography, logos, and product graphics may require compositing or manual retouching.

## Boundaries

- Produce an original interpretation; do not reproduce a specific frame, character design, dialogue, subtitle, or film asset.
- Do not present results as official film material or imply affiliation.
- Do not remove watermarks or ownership marks.
- Do not identify a real person from an image.
- Keep user constraints above the default style system.

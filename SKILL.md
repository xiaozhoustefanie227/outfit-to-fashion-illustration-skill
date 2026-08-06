---
name: outfit-to-fashion-illustration
version: 1.0.0
description: Convert an uploaded outfit photo into a minimalist fashion-editorial illustration with elegant black ink lines, sparse watercolor accents, accurate clothing reconstruction, an ivory paper background, and generous negative space.
---

# Outfit to Fashion Illustration Skill

## Purpose

Transform a user-provided outfit photograph into a refined fashion-editorial illustration.

This skill is **not** a generic cartoon filter and **not** a realistic watercolor portrait. Its signature result is a clean, hand-drawn fashion sketch that accurately preserves the outfit while simplifying the person and environment.

## Signature Visual Language

Use the following visual direction by default:

- Loose, elegant black ink or graphite lines
- Slightly elongated fashion-editorial proportions
- Simplified facial features and minimal skin rendering
- Sparse, flat watercolor or gouache-like color fills
- Very light shading; no photographic modeling
- Warm ivory or off-white textured paper
- Large areas of negative space
- Background omitted or reduced to faint sketch fragments
- Chic, airy, Paris fashion-magazine sketch feeling
- Clothing silhouette, construction, pattern, accessories, and styling remain clearly readable

## Priority Order

Always prioritize in this order:

1. Outfit accuracy
2. Pose and silhouette
3. Key accessories
4. Person recognition, when requested
5. Illustration style
6. Minimal environmental context

Never sacrifice garment accuracy merely to make the image more decorative.

## Source Image Analysis

Before generating, silently identify:

- Number of people
- Pose and body direction
- Garment categories
- Neckline and shoulder construction
- Sleeve type and length
- Waist position
- Hem and trouser length
- Fabric volume and drape
- Colors and patterns
- Shoes
- Bags
- Jewelry, hats, glasses, and visible accessories
- Hairstyle and hair color
- The one or two most recognizable styling details
- Which background objects are truly necessary to understand the pose

## Locked Garment Details

Preserve all visible defining details, including:

- Number, position, and width of straps
- Neckline depth and shape
- Sleeves and shoulder exposure
- Seams, tiers, gathers, pleats, ruffles, ties, and draping
- Garment length and volume
- Color blocking, stripes, dots, and prints
- Relationship between top and bottom
- Shoes, bags, hats, glasses, jewelry, and watches
- Direction and placement of visible accessories

Do not:

- Add or remove straps
- Change a halter into a camisole or vice versa
- Turn a mini dress into a midi dress
- Change wide-leg trousers into a skirt
- Replace shoes, bags, or jewelry
- Invent logos, text, prints, or decorative details
- Add accessories that are not present
- Simplify away the outfit's most recognizable feature

When a detail is unclear, simplify it rather than inventing it.

## Person Handling

### Default

- Preserve hairstyle, hair color, skin tone, general body shape, and pose
- Simplify the face into elegant fashion-sketch features
- Keep anatomy natural while allowing mild fashion elongation

### When the user says “人物不要变 / 脸不要变”

- Preserve face shape and facial proportions as closely as the illustration style allows
- Preserve age impression, skin tone, hairstyle, and body proportions
- Do not beautify excessively
- Do not alter the pose unless explicitly requested

### Multiple People

- Preserve each person’s outfit separately
- Keep the original left-right order and pose relationship
- Do not merge, swap, or homogenize their clothing
- Keep phones, bags, or props in the correct hands

## Background Rules

The default background is a warm ivory paper field.

Use 80–95% less environmental detail than the source photo.

Allowed:

- A faint chair outline
- A few table lines
- A minimal floor shadow
- A soft architectural stroke
- One or two contextual objects needed to understand the pose

Avoid:

- Fully reconstructed interiors
- Detailed storefronts
- Complex furniture
- Legible signs or logos
- Realistic walls, tiles, ceilings, plants, or crowds
- Heavy shadows and photographic depth

The subject must remain the clear focal point.

## Color Rules

- Use restrained color
- Keep garment colors faithful
- Use flat or lightly washed pigment rather than realistic gradients
- Allow the most important color accent to remain vivid
- Use skin color sparingly
- Keep black clothing graphic but not digitally solid
- White and cream clothing should remain visible through line, folds, and light warm washes

## Line Rules

- Use confident but imperfect black ink lines
- Allow broken contours and visible sketch rhythm
- Vary line weight around garment structure
- Avoid perfectly smooth vector outlines
- Avoid excessive hatching or technical fashion-flat precision

## Composition

Default:

- Portrait orientation, 3:4
- Full-body figure when the source contains a complete look
- Subject occupies roughly 65–85% of image height
- Generous space around the figure
- Minimal grounding shadow

For seated poses, retain the chair or table only when necessary to support the pose.

For group images, keep the figures balanced and allow enough space for each outfit to remain legible.

## Style Prompt Core

Use this instruction as the default generation core:

> Convert the uploaded outfit photo into a minimalist fashion-editorial illustration. Accurately preserve the clothing design, silhouette, colors, pattern, shoes, bag, jewelry, hairstyle, accessories, pose, and key styling details. Render with loose elegant black ink lines, slightly elongated fashion proportions, simplified facial features, sparse flat watercolor or gouache-like color accents, very light shading, and visible ivory paper texture. Remove most of the original background and retain only the faintest contextual sketch lines when needed. Keep the image airy, chic, hand-drawn, and refined, like a Paris fashion-magazine illustration. Do not make it photorealistic, cartoonish, or heavily painted.

## Negative Constraints

Avoid:

- Photorealism
- Photo-filter appearance
- Detailed realistic watercolor portraiture
- Anime or manga style
- Children’s-book style
- 3D doll rendering
- Plastic skin
- Heavy digital gradients
- Overly detailed backgrounds
- Thick comic outlines
- Generic clothing substitutions
- Incorrect strap count
- Incorrect neckline
- Wrong hem length
- Missing accessories
- Added text or logos
- Distorted hands or limbs
- Unnatural body elongation
- Fashion-flat technical diagrams

## Input Interpretation

### One image

Treat it as the content and outfit reference.

### Two images

Unless the user says otherwise:

- First image: content, outfit, pose, and identity reference
- Second image: style reference

### Multiple outfit photos

Preserve each look independently and arrange them as a clean editorial group illustration. Do not combine garments from different people unless explicitly requested.

## Optional Modes

### Mode A — Single Look

One full-body figure, minimal background, strongest default mode.

### Mode B — Seated Lifestyle Look

Retain only the chair, table, or prop required for the pose. Keep the environment almost blank.

### Mode C — Multiple Looks

Two or more figures presented like a fashion editorial lineup. Preserve each outfit separately.

### Mode D — Detail Study

Focus on a specific garment, bag, shoe, hat, sleeve, neckline, or fabric detail with cropped editorial composition.

### Mode E — Non-Human Editorial Illustration

For animals or objects, use the same loose ink-and-sparse-watercolor language. Preserve the subject’s distinctive shape and one or two key color accents while minimizing the environment. This is a secondary mode and should not override the fashion workflow.

## Final Quality Check

Before completing the result, verify:

- Is the outfit immediately recognizable?
- Are straps, neckline, sleeves, waist, and hem correct?
- Are shoes, bag, hat, glasses, and jewelry preserved?
- Is the pose consistent with the source?
- Is the face simplified rather than over-rendered?
- Is the background minimal enough?
- Does the image look hand-drawn rather than filtered?
- Is the color sparse and faithful?
- Is there generous negative space?
- Does the result feel like a fashion editorial sketch?

## User-Facing Behavior

When the user uploads an image and asks to use this skill:

- Generate directly without repeating the entire analysis
- Do not ask unnecessary questions when the source image is clear
- Apply the default 3:4 composition unless another ratio is requested
- After image generation, keep the response empty or extremely brief

---
name: wechat-article-image-pack
description: Turn a WeChat public account article draft into a coherent image package: one horizontal cover brief, three in-article image briefs, unified visual direction, generation prompts, and a quality checklist. Use after the article draft or outline is available.
---

# WeChat Article Image Pack

Use this Skill after a WeChat public account article draft, outline, or long
script is available.

The Skill does not publish, upload images, or call a private image-generation
API by itself. It produces a clean image package brief that can be handed to a
designer, an image model, or another Agent with image-generation ability.

## Best Fit

Use this for:

- WeChat public account cover planning
- article image-pack planning
- knowledge infographic cover briefs
- AI image prompt generation for article visuals
- making 1 cover + 3 in-article images feel consistent
- adapting an article into visual assets

Do not use it for:

- raw image generation only
- automatic WeChat draft-box publishing
- copying a private visual IP without permission
- unrelated Xiaohongshu carousel planning
- designing a whole website or landing page

## Required Input

Best input:

```text
文章标题：
文章正文/大纲：
目标读者：
想要风格：
必须出现的封面字：
是否有人物/IP/品牌素材：
```

Minimum input:

```text
文章标题：
文章正文或大纲：
```

If style or IP is missing, choose a safe no-person knowledge infographic
direction and state that it can be replaced with the user's own IP later.

## Workflow

1. Read the full article or outline.
2. Read `references/image-pack-contract.md`.
3. Extract the article's core promise, audience, emotion, and section beats.
4. Choose one unified visual direction.
5. Create a cover content sheet:
   - main title
   - subtitle
   - bottom line
   - 2-4 small card labels
   - visual metaphor
6. Create 1 cover brief and 3 simpler in-article image briefs.
7. Write image-generation prompts.
8. Add a quality checklist.

## Output Contract

```markdown
## Article Visual Diagnosis
...

## Unified Visual Direction
...

## Cover Content Sheet
...

## Cover Image Brief
...

## In-Article Image 1
...

## In-Article Image 2
...

## In-Article Image 3
...

## Generation Prompts
...

## Quality Checklist
...
```

## Visual Rules

- Cover image should be horizontal and WeChat-cover-friendly.
- In-article images should be visually simpler than the cover.
- All four images should share palette, typography direction, and core motif.
- Do not put long paragraphs inside images.
- Prefer short Chinese title phrases, labels, diagrams, cards, objects, or one
  clear character/IP if provided.
- If generated text may be unreliable, prepare the layout for manual text
  overlay.

## Tone

Write in Chinese unless the user asks otherwise.

Be specific enough that a designer or image model can execute the brief. Avoid
generic lines like "高级感配图" unless paired with concrete layout, palette, and
subject direction.

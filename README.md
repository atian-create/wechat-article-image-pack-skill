# WeChat Article Image Pack Skill

Turn a WeChat public account article draft into a small visual package:

- 1 horizontal WeChat cover image brief
- 3 in-article image briefs
- unified visual direction
- image-generation prompts
- quality checklist

这个开源 Skill 解决的是公众号写完以后最容易卡住的一步：

> 文章已经有了，但封面和正文配图还要重新想，风格还容易乱。

It is not an image-generation API. It is a connector-neutral planning and
briefing Skill that helps an Agent or creator turn article text into a coherent
image package.

## Search Keywords

English keywords:

`WeChat article cover`, `WeChat public account images`, `article image pack`,
`knowledge infographic cover`, `AI image prompt`, `creator workflow`,
`newsletter image brief`, `content design`, `visual content system`,
`AI skill for creators`.

中文关键词：

`公众号封面`, `微信公众号封面`, `公众号配图`, `公众号正文插图`,
`文章配图`, `知识信息图封面`, `AI 生图提示词`, `公众号视觉系统`,
`创作者工具`, `内容工作流`, `封面 brief`.

## Why This Exists

公众号文章的配图不是单张图问题，而是整篇文章的视觉统一问题。

This Skill reads the article draft first, then extracts:

- article promise
- main title and subtitle
- core sections
- visual metaphor
- cover text
- in-article image beats
- style direction
- generation-ready prompts

## What It Can Do

- turn an article draft into a cover content sheet
- design one WeChat-cover-friendly horizontal cover brief
- design three simpler in-article image briefs
- keep all four images visually consistent
- support a no-person knowledge infographic style
- support a recurring creator character/IP style when the user provides one
- support replacing the visual IP with the user's own brand assets
- produce prompts for image-generation tools

## Open-Source Boundary

This open version includes:

- article-to-image-pack workflow
- cover content extraction rules
- image-pack output contract
- prompt structure
- quality checklist
- sample input and output

This open version does not include:

- private article libraries
- WeChat draft-box API
- image-generation API keys
- private brand assets
- paid connector logic
- automatic publishing

If an image-generation tool is available, an Agent can use the generated prompts
to create files. If no tool is available, this Skill still produces a usable
designer/model brief.

## Best Inputs

- WeChat article title
- full article draft
- article outline
- target audience
- desired style
- brand color or IP reference
- must-use cover words
- optional reference images

## Output Contract

Default output:

1. Article visual diagnosis
2. Unified visual direction
3. Cover content sheet
4. Cover image brief
5. In-article image 1 brief
6. In-article image 2 brief
7. In-article image 3 brief
8. Generation prompts
9. Quality checklist

## Example Prompts

```text
把这篇公众号稿做成一套配图 brief：1 张封面 + 3 张正文插图。
```

```text
这篇文章是 AI 工作流主题，帮我提炼封面标题、视觉隐喻和 3 张正文图提示词。
```

```text
我有自己的卡通 IP，帮我把文章配图做成统一风格，但不要自动发布。
```

## Repository Map

- `SKILL.md`: Agent entrypoint and workflow rules
- `agents/openai.yaml`: OpenAI Agent display metadata
- `references/image-pack-contract.md`: detailed output contract
- `examples/sample-image-pack.md`: sample package

## Recommended GitHub Description

> Open Skill for turning WeChat public account articles into a cover plus three coherent in-article image briefs and prompts.

## Suggested GitHub Topics

`wechat`, `wechat-public-account`, `article-cover`, `image-prompt`,
`content-design`, `creator-tools`, `ai-skill`, `visual-content`,
`knowledge-infographic`, `newsletter`

## License

MIT

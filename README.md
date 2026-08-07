# AgentDock Prompt Library

Source files for the [AgentDock Prompt Library](https://agentdock.ai/prompt-library).
Every prompt on the site lives here as an MDX file, one file per prompt,
organized by category. The library keeps growing, and this repository is
always the source.

## How a prompt works

Open any file. The top is frontmatter, the rest is the prompt itself. The parts
you fill in are wrapped in brackets:

```text
I need to create an action plan for this goal: [GOAL_DESCRIPTION]

The timeframe for completion is [TIMEFRAME:select:1 week,2 weeks,1 month,3 months,6 months,1 year]
```

Swap the brackets for your own details and paste the whole thing into a chat.
A plain `[VARIABLE]` takes free text. A `select` variable lists the values it
expects.

Most files carry demo links in their frontmatter: the same prompt already run
in ChatGPT, Claude, Perplexity, and Qwen, so you can read real output before
you spend your own tokens.

## Layout

Each folder is a category, each file is a prompt. The path is the page:
`business/action-plan-generator.mdx` lives at
[agentdock.ai/prompt-library/business/action-plan-generator](https://agentdock.ai/prompt-library/business/action-plan-generator).

## Frontmatter

| Field | What it holds |
|-------|---------------|
| `title`, `description` | What the prompt does |
| `slug` | Category and page path |
| `tags` | Search and related-prompt matching |
| `agentdockUrl` | The hosted page for this prompt |
| `chatgptDemoUrl`, `claudeDemoUrl`, ... | Example runs in ChatGPT, Claude, Perplexity, and Qwen |

## License

[CC BY 4.0](./LICENSE). Use the prompts anywhere, including commercially.
Copies and adaptations must credit AgentDock and link back to this repository
or [agentdock.ai/prompt-library](https://agentdock.ai/prompt-library).

---

These files moved here from [AgentDock/AgentDock](https://github.com/AgentDock/AgentDock)
with their commit history intact.

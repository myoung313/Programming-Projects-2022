# Digital Products Workspace

Four Claude Code subagents (in `.claude/agents/`) run the product pipeline:

| Step | Agent | Ask Claude… | Writes to |
|---|---|---|---|
| 1 | `trend-researcher` | "Use trend-researcher on 2027 budget spreadsheets" | `research/` |
| 2 | `design-remixer` | "Use design-remixer on the newest brief" | `designs/<product>/spec.md` |
| 3 | `listing-writer` | "Use listing-writer for <product>" | `listings/<product>.md` |
| 4 | `funnel-builder` | "Use funnel-builder for <product>" | `funnels/<product>/` (funnel plan + landing page) |

Or run the whole pipeline at once: *"Run the product pipeline for <niche>."*

Every product must pass design-remixer's originality check, and any product made with AI help needs the AI disclosure on its Etsy listing.

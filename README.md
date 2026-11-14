# Claude skills by Muzeeb Urrahaman

Eight Claude skills for design review, UX, writing and brand work, each benchmarked against plain Claude and the closest comparable skill.

| Skill | No skill | Comparable skill | v1.0 | v1.1 |
|---|---|---|---|---|
| [honest-review](honest-review) | 64% | design-critique: 68% | 100% | **100%** |
| [ux-assistant](ux-assistant) | 69% | accessibility-auditor: 77% | 100% | **100%** |
| [portfolio-review](portfolio-review) | 75% | design-critique: 79% | 92% | **92%** |
| [antislop-content](antislop-content) | 75% | stop-slop: 92% | 92% | **92%** |
| [antislop-ui](antislop-ui) | 100% | impeccable: 100% | 100% | **98%** |
| [fact-checker](fact-checker) | 85% | deep-research: 85% | 92% | **98%** |
| [user-flow-creator](user-flow-creator) | 50% | ux-flow-designer: 11% | 42% | **83%** |
| [brandkit-deck](brandkit-deck) | 64% | ui-ux-pro-max · brand: 86% | 86% | **86%** |

Each skill has two test cases in its `evals/` folder, run with `claude plugin eval` in clean sessions and graded against written checks. Details and per-case scores are on each skill's page at https://muzeeb-design.vercel.app/skills

| Skill | What it does |
|---|---|
| [honest-review](honest-review) | Design review with a verdict and findings ranked Blocker to Nit |
| [ux-assistant](ux-assistant) | UX and WCAG 2.2 AA audit with measured values and code fixes |
| [portfolio-review](portfolio-review) | Reads a case study the way a hiring manager does, then ranks the fixes |
| [antislop-content](antislop-content) | Removes AI writing patterns and keeps every fact |
| [antislop-ui](antislop-ui) | Finds AI-default UI and rebuilds the page around the product |
| [fact-checker](fact-checker) | Checks claims one by one, with a source for every verdict |
| [user-flow-creator](user-flow-creator) | 50% | ux-flow-designer: 11% | 42% | **83%** |
| [brandkit-deck](brandkit-deck) | Builds a brand kit and a matching 10-slide deck from a logo and theme |

Each skill has a page with demos at https://muzeeb-design.vercel.app/skills

## Install

**Claude Code** (replace the name with the skill you want):

```bash
mkdir -p ~/.claude/skills && curl -fsSL https://github.com/MUZEEBURRAHAMAN/claude-skills/raw/main/dist/honest-review.zip -o /tmp/honest-review.zip && unzip -oq /tmp/honest-review.zip -d ~/.claude/skills/
```

**Claude.ai:** download the zip from [`dist/`](dist) and upload it under Settings → Capabilities → Skills.

## Tests

Each skill folder has an `evals/` folder with one test case: the prompt, the input files and the checks a grader used. The cases use the layout `claude plugin eval` reads, so you can run them yourself.

## License

MIT

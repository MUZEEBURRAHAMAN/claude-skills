# Claude skills by Muzeeb Urrahaman

Eight Claude skills for design review, UX, writing and brand work. Each one was tested on a realistic task against plain Claude. With the skill, the runs passed 49 of 50 checks. Without it, they passed 36 of 50.

| Skill | What it does |
|---|---|
| [honest-review](honest-review) | Design review with a verdict and findings ranked Blocker to Nit |
| [ux-assistant](ux-assistant) | UX and WCAG 2.2 AA audit with measured values and code fixes |
| [portfolio-review](portfolio-review) | Reads a case study the way a hiring manager does, then ranks the fixes |
| [antislop-content](antislop-content) | Removes AI writing patterns and keeps every fact |
| [antislop-ui](antislop-ui) | Finds AI-default UI and rebuilds the page around the product |
| [fact-checker](fact-checker) | Checks claims one by one, with a source for every verdict |
| [user-flow-creator](user-flow-creator) | Draws user flows as HTML pipelines, current vs proposed |
| [brandkit-deck](brandkit-deck) | Builds a brand kit and a matching 10-slide deck from a logo and theme |

Each skill has a page with demos at https://muzeeb-portfolio-v2.vercel.app/skills.html

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

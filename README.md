# Funnel Landing Skill

An agent skill for planning conversion funnels, writing landing pages, and reviewing connected campaign journeys. It combines the **4 Cs**—Captivate, Curiosity, Convince, Convert—with **Hook–Story–Offer** and a practical model for audience, outcomes, objections, mechanisms, evidence, and next actions.

## Install

```bash
npx skills add matteolaureti/funnel-landing-skill --skill funnel-landing-strategy
```

For Codex in the current project:

```bash
npx skills add matteolaureti/funnel-landing-skill --skill funnel-landing-strategy --agent codex
```

Add `--global` to make it available across projects. The CLI may offer agent and installation-method choices. See the [official CLI documentation](https://github.com/vercel-labs/skills).

Inspect discovery without installing:

```bash
npx skills add matteolaureti/funnel-landing-skill --list
```

Skills.sh lists skills through installation telemetry; a compatible GitHub repository does not by itself establish that a skill has appeared in the directory. See the [listing FAQ](https://skills.sh/docs/faq#how-do-i-get-my-skill-listed-on-the-leaderboard).

## Use

Invoke `$funnel-landing-strategy` in Codex, or use your agent's invocation mechanism. The skill follows the user's language.

> Use $funnel-landing-strategy to plan a direct-sale funnel for this product. Explain the path, evidence each page needs, and what happens after purchase.

> Use $funnel-landing-strategy to write a landing page for this free resource and explain how it connects to our paid offer. Separate confirmed facts from assumptions.

> Use $funnel-landing-strategy to review our demo-booking journey. Identify gaps in promise, evidence, booking, and follow-up; prioritize changes.

You can ask in Italian or another language supported by the agent. Supply existing offer, audience, entry messages, evidence, terms, pages, or data when available. The skill asks for consequential missing information rather than a mandatory questionnaire.

## Working modes

- **Plan:** brief, reasoned path, central message, page specifications, evidence gaps, and measurement hypotheses.
- **Write:** requested structure and copy using a defined strategy.
- **Review:** concrete findings, implications, and prioritized changes within available evidence.

The 4 Cs describe journey functions; they do not require four pages or sections. The skill distinguishes local conversions from final business outcomes and chooses intermediate steps according to the uncertainty they resolve.

The scope is strategy, messaging, and page handoff. Coding, analytics setup, campaign execution, and publication depend on the user's request and available tools. No particular framework, connector, or runtime is required to use the skill.

## Contents

```text
skills/funnel-landing-strategy/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── funnel-patterns.md
    ├── messaging-and-story.md
    ├── project-brief.md
    ├── review-criteria.md
    └── worked-examples.md
```

References are read as needed. Codex UI metadata is optional for other agents; core instructions are portable Markdown with YAML frontmatter.

## Evaluation

Version **0.1.0** includes hypothetical walkthroughs for direct purchase, a resource leading to a course, and a B2B demo. Each has a changed condition to check adaptation. They support conceptual review, not claims of observed conversion performance.

See [evaluation scenarios](docs/evaluation.md) for repeatable behavioral checks. These are instructions, not a claim that independent agent tests have passed. Evaluate audience understanding and commercial results on a real project before making performance claims.

## Sources

- [The Only Marketing Strategy You Need to Make $1,000,000](https://www.youtube.com/watch?v=ab6H-9fxlPI), the video behind the supplied transcript that inspired the 4 Cs discussion.
- [Hook–Story–Offer, ClickFunnels](https://www.clickfunnels.com/blog/hook-story-offer/).
- [Principles of persuasion, Cialdini](https://www.influenceatwork.com/7-principles-of-persuasion/).
- [Agent Skills specification](https://agentskills.io/specification).
- [Skills CLI](https://github.com/vercel-labs/skills).

This skill combines the 4 Cs with an original operational decision model and page workflow developed from that discussion. The source transcript is not included. References do not imply endorsement or guarantee outcomes.

## License

[MIT](LICENSE).

# Funnel Landing Skill

Create landing pages and campaign content using the **4 Cs**—Captivate, Curiosity, Convince, Convert. Ground the customer's **Story** in project context: **Identify** who they are, the **Outcome** they want, and the **Objection**—an experience or consequence they want to avoid in their current way of pursuing that outcome, before introducing the product.

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

> Use $funnel-landing-strategy to create a landing page for this product. Build the funnel context from the supplied information and write in English.

> Use $funnel-landing-strategy to write social content for this campaign using our existing funnel-context.md. Write in English.

> Use $funnel-landing-strategy to review this landing page against our funnel context. Explain where its message or progression needs work.

You can ask in Italian or another language supported by the agent. Supply existing offer, audience, entry messages, supporting material, terms, pages, or data when available.

## Scope

The method applies to landing pages, social posts, ads, videos, emails and connected campaigns. Ask for the content, plan, review or implementation you need.

The 4 Cs describe a progression, not four compulsory sections. A function can continue across several passages, and one passage can serve several functions. Format, length, commercial action and page structure come from the project rather than a catalogue of funnel patterns.

Implementation and publication depend on the user's request and available tools. No particular framework, connector, or runtime is required.

## Contents

```text
skills/funnel-landing-strategy/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── funnel-context.md
    └── messaging-and-story.md
```

References are read as needed. Codex UI metadata is optional for other agents; core instructions are portable Markdown with YAML frontmatter.

| Reference | Purpose |
|---|---|
| [Funnel context](skills/funnel-landing-strategy/references/funnel-context.md) | Create and maintain a project Markdown document with audience, desired outcomes, experiences to avoid, offer, capabilities and supporting material. |
| [Messaging and story](skills/funnel-landing-strategy/references/messaging-and-story.md) | Connect those elements throughout the 4 Cs, using features, demonstrations and customer experiences to develop the customer's Story. |

## Evaluation

Version **0.4.3** explains the funnel, the Story and their project context as distinct parts of the method. Its two references cover reusable project-context documentation and the customer's Story, without a funnel-pattern catalogue or separate communication and review guides.

See [evaluation scenarios](docs/evaluation.md) for repeatable behavioral checks.

## Sources

- [The Only Marketing Strategy You Need to Make $1,000,000](https://www.youtube.com/watch?v=ab6H-9fxlPI), the video behind the supplied transcript that inspired the 4 Cs discussion.
- [What is a marketing funnel?, Whop](https://whop.com/blog/what-is-a-marketing-funnel/).
- [Rethinking skills and prompts for GPT-6 Astra, OpenAI](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra), informing the compact entrypoint and selective references.
- [Agent Skills specification](https://agentskills.io/specification).
- [Skills CLI](https://github.com/vercel-labs/skills).

This skill's application throughout content and its reusable project context are an operational interpretation of the cited guidance. The source transcript is not included.

## License

[MIT](LICENSE).

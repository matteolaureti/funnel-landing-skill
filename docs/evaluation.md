# Behavioral evaluation scenarios

These prompts are inputs for future agent checks of version 0.4.3. Give the agent a prompt and the skill in an isolated project, without the assessment criteria. Keep generated artifacts local.

## Landing page and saved context

**Prompt:**

> Use funnel-landing-strategy to create a local English HTML landing page for this hypothetical business: ShiftPlan, software for restaurant managers to record staff availability and plan weekly shifts. Managers currently compare availability messages with a separate schedule. The software shows recorded availability alongside planned shifts. Its monthly plan costs €29. There are no supplied customer results, automatic conflict alerts or integration details. We want visitors to buy the monthly plan. Work only in this project directory and do not publish externally.

**Assess:** a reusable Markdown context document records the audience, desired outcomes, experiences to avoid, offer, capabilities and supporting material; Identify describes a recognizable situation; Outcome explains a desired result; Objection comes from the managers' current scheduling process, such as last-minute calls after availability was missed in messages. Questions about adopting the software are recorded separately. Features develop those connections. The 4 Cs develop the content without a mandatory section count.

## Reuse for another format

**Prompt:**

> Use funnel-landing-strategy and the project's existing funnel-context.md to write an English social post for the same product. The intended action is to visit its landing page. Save the draft locally.

**Assess:** the existing context is reused; the story and action fit the new format; the output does not default to a four-block page or an unrelated commercial pattern.

## Update the context

**Prompt:**

> Use funnel-landing-strategy to revise this project's context and landing-page copy. We have confirmed that managers enter staff availability themselves; staff do not have accounts. Keep the rest of the supplied product facts and terms.

**Assess:** the context records the updated process; the copy reflects how managers enter availability and uses that context to develop the Story.

## Record results

Record the skill version, model, prompt, generated context and content, observed strengths and misses. Separate structural checks, model behavior, actual audience understanding and commercial performance.

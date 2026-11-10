# Claude Bleu Skill

A structured system-planning skill for turning an idea into a complete, production-ready implementation blueprint before code is written. Bleu organizes project discovery, architecture, decisions, execution details, and validation into a persistent, navigable planning workspace.

## What It Covers

- **Project discovery:** Clarify goals, constraints, stakeholders, and success criteria.
- **System architecture:** Break a concept into components, services, data flows, and integrations.
- **Implementation planning:** Translate the architecture into actionable work and file-level execution.
- **Persistent planning workspace:** Maintain linked planning documents and session state across work sessions.
- **Quality and linting:** Review each planning phase for missing decisions, gaps, and inconsistencies.
- **Research:** Incorporate web research into the planning process as required by the skill.
- **Advanced patterns:** Support living knowledge bases, reflection loops, multi-agent workflows, and schema-driven planning.

## Installation

Clone this repository into your Claude skills directory:

```bash
git clone https://github.com/Brajesh31/claude-bleu-skill.git ~/.claude/skills/bleu
```

## Using the Skill

Example request:

```text
Use the bleu skill to blueprint a production-ready SaaS platform.
Map the architecture, components, data flows, implementation phases,
risks, and file-level execution plan before coding.
```

Bleu is intended for substantial planning work. It creates a structured workspace rather than returning only a one-off architecture summary. Use its resume triggers and workspace files to continue a plan across sessions.

## Workflow and Workspace

The skill defines a phased process for gathering requirements, researching, designing the system, mapping implementation, and linting the resulting plan. It describes workspace artifacts such as `SESSION.md`, `NEXT.md`, and decision records to preserve context.

## Repository Resources

- [SKILL.md](SKILL.md) contains the full planning workflow and operating rules.
- `references/` contains supporting guidance for the workflow and workspace.

## Good Practices

Treat the blueprint as a decision record, not a substitute for validating assumptions. Keep requirements, research findings, trade-offs, and unresolved questions explicit. Update the workspace as architecture decisions or project constraints change.

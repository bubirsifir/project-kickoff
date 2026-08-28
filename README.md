# Project Kickoff

Project Kickoff is an adaptive discovery skill for ChatGPT and Codex. It turns an early idea, new product request, or material change to an existing project into an approved `PROJECT-BRIEF.md` before implementation begins.

It does not make users complete a long form. It inspects what is already known, asks one high-impact question at a time, explains tradeoffs, recommends a direction, and skips irrelevant branches.

## What it covers

- Idea, user, problem, value, business model, and success measures
- Website, SaaS, mobile, ecommerce, AI, automation, API, and existing-project routes
- Responsive web, PWA, iOS, Android, desktop, API, and multi-surface platform decisions
- MVP scope, roles, flows, brand, content, architecture, data, integrations, and AI behavior
- Security, privacy, accessibility, operations, rollout, risks, and acceptance criteria
- A living decision log and explicit approval gate before implementation

## Example

Invoke the skill and describe the idea in any language:

```text
Use $project-kickoff. I want to build an AI-assisted appointment product for small businesses, but I have not decided whether it should be web-only or web plus mobile.
```

The skill first classifies the project and its maturity, then asks only the decisions that affect the next phase. It writes or updates `PROJECT-BRIEF.md` when file changes are authorized and waits for approval before implementation.

## Install as a plugin from GitHub

Add the public GitHub marketplace:

```bash
codex plugin marketplace add bubirsifir/project-kickoff
codex plugin add project-kickoff@project-kickoff
```

Start a new conversation after installation, then invoke `$project-kickoff` or describe a new project naturally.

## Install as a standalone skill

Copy the skill directory into your personal skills folder:

```bash
mkdir -p ~/.agents/skills
cp -R plugins/project-kickoff/skills/project-kickoff ~/.agents/skills/project-kickoff
```

For one repository only, copy it to:

```text
<repository>/.agents/skills/project-kickoff
```

Codex can also install skills from other repositories through `$skill-installer`.

## Repository structure

```text
.agents/plugins/marketplace.json
plugins/project-kickoff/
  .codex-plugin/plugin.json
  skills/project-kickoff/
    SKILL.md
    agents/openai.yaml
    references/
    assets/PROJECT-BRIEF.template.md
```

## Design principles

- Adaptive interview, not a static questionnaire
- One material decision at a time
- User intent decisions separated from agent implementation decisions
- Product need before framework choice
- Explicit platform and product-surface mapping
- Progressive disclosure to keep context efficient
- Visible assumptions, conflicts, risks, and deferred work
- Approval before implementation

## Compatibility

The skill follows the open Agent Skills directory format. The plugin wrapper provides the recommended installable distribution unit for ChatGPT and Codex. Hosts that support standalone agent skills can use the inner `skills/project-kickoff` folder directly.

## Contributing

Test changes with realistic project prompts. Prefer narrow improvements based on observed failures over adding universal questions. Keep `SKILL.md` focused and place conditional guidance in `references/`.

## License

MIT

---

## Türkçe kısa açıklama

Project Kickoff, kullanıcıya uzun bir form doldurtmadan yeni proje fikrini profesyonel bir başlangıç görüşmesiyle netleştirir. Proje türüne göre sorularını uyarlar, web/mobil/platform kararlarını erkenden belirler, kararları `PROJECT-BRIEF.md` içinde tutar ve kullanıcı onayı olmadan geliştirmeye başlamaz.

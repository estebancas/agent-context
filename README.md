### Agent specific markdown files

This is a folder architecture template to improve agent project context and token efficiency

The main idea is to divide most common workflows or relevant sections of the app and create a CONTEXT.md, and use CLAUDE.md/AGENTS.md as the floor plan to briefly point every important aspect of the project.

```
my-app/
├── CLAUDE.md
├── planning/
│   ├── CONTEXT.md
│   ├── specs/
│   ├── architecture/
│   └── decisions/
├── src/
│   ├── CONTEXT.md
│   ├── components/
│   ├── services/
│   ├── utils/
│   └── tests/
├── docs/
│   ├── CONTEXT.md
│   ├── api/
│   ├── guides/
│   └── changelog/
└── ops/
    ├── CONTEXT.md
    ├── deploy/
    ├── monitoring/
    └── scripts/
```

**What each workspace does:**

<u>Planning</u>: Specs, architecture decisions, design docs. The CONTEXT.md describes the app, the tech stack, current priorities and any architectural principle I follow. This is what claude will read when I tell to help spect a new feature.

<u>src</u>: Actual code base. The CONTEXT.md here describes the code structure, naming conventions, patterns you use (and what patterns to avoid), testing requirements, and libraries or frameworks that are standard in the project.

<u>docs</u>: API documentation, user guides. The CONTEXT.md describes project documentation standards, the audience for each type of doc, and how docs are related to the code

<u>ops</u>: Deployment, monitoring, operational scrips. The CONTEXT.md describes the infrastructure, deploy process and any runbook convention.


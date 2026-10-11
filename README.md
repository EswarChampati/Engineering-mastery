# 180-Day Engineer Transformation

A hands-on engineering roadmap focused on JavaScript/TypeScript, backend systems, cloud-native engineering, platform engineering, distributed systems, and applied AI/LLM systems.

## Goals

Over 180 days, build practical skills and portfolio evidence through small exercises, tested projects, architecture decisions, debugging notes, and documented trade-offs.

The goal is to become capable of designing, implementing, testing, operating, and explaining production-minded systems. Completing a roadmap does not guarantee a particular role or compensation; outcomes depend on demonstrated skills, interviews, and market conditions.

## Start here

1. Read [`ROADMAP.md`](ROADMAP.md) for the sequence and milestones.
2. Read [`PROGRESS.md`](PROGRESS.md) and update it at the end of each study day.
3. Complete [`day-000-js-ts-git-reset/README.md`](day-000-js-ts-git-reset/README.md) before starting Day 1.
4. Keep each day’s code, tests, and notes in the appropriate day or project folder.
5. Commit meaningful changes and push them to GitHub.

## Repository map

```text
180-day-engineer-transformation/
├── README.md
├── ROADMAP.md
├── PROGRESS.md
├── .gitignore
├── day-000-js-ts-git-reset/
│   ├── README.md
│   ├── javascript/
│   ├── typescript/
│   ├── git-lab/
│   └── notes/
├── month-01-nodejs-typescript-backend/
├── month-02-data-and-messaging/
├── month-03-cloud-and-cicd/
├── month-04-kubernetes-and-platform/
├── month-05-distributed-systems-and-ai/
├── month-06-capstone-and-interviews/
├── docs/
│   ├── architecture/
│   ├── adr/
│   ├── interview-notes/
│   ├── system-design/
│   └── retrospectives/
└── templates/
    ├── daily-log.md
    ├── project-readme.md
    ├── adr.md
    └── incident-review.md
```

Create daily folders as you reach them; do not create empty folders just to fill the tree. Put integrated projects under the relevant month’s `projects/` directory and link to them from daily notes.

## Daily engineering loop

- Learn the concept and explain it in your own words.
- Predict output or behavior before running the code.
- Implement the task without copying a solution line by line.
- Test normal cases, edge cases, and failure paths.
- Record mistakes, debugging steps, and lessons learned.
- Commit and push a meaningful increment.
- Update `PROGRESS.md`.

## Working agreements

- Use `main` as the stable branch and short-lived branches for meaningful changes.
- Prefer small, focused commits with clear messages (`feat:`, `fix:`, `test:`, `docs:`, `refactor:`, `chore:`).
- Never commit passwords, tokens, private keys, real `.env` values, or employer-confidential material.
- Use a disposable repository to practise destructive Git commands.
- Prefer `git revert` for undoing a commit already shared with others. Understand the effects before using `git reset --hard`, rewriting history, or force-pushing.
- Document important design choices in `docs/adr/`.
- A checkbox means completed only when you have evidence.

## Definition of done for a study day

- [ ] I can explain the key ideas without notes.
- [ ] I completed the hands-on task myself.
- [ ] I ran relevant tests or verification commands.
- [ ] I recorded at least one lesson, mistake, or question.
- [ ] I committed and pushed the work.
- [ ] I updated `PROGRESS.md`.

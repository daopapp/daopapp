## Rodrigo Papp

Senior Full-Stack Engineer and Tech Lead, 18 years. Seven of them building production PHP with Laravel and Symfony, paired with TypeScript front ends in React, Next.js and Vue. My track record is modernising legacy PHP: introducing React and Vite architectures into codebases that had none, and shipping features that go all the way through, from API design and data modelling to component architecture and CI.

I started on IBM mainframe, writing COBOL, DB2 and JCL for telecom and insurance systems with 24/7 production support. That is where I learned what a bad deploy costs, and I have not needed to relearn it since.

Currently leading the engineering and AI teams of an automation platform on Google Cloud. Most of that work is private, so the repository list here is smaller than the contribution graph.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rodrigo-papp-cadima/)
[![Email](https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=white)](mailto:daopapp@gmail.com)

---

### Open source

**[copybook-ts](https://github.com/daopapp/copybook-ts)** &nbsp;·&nbsp; TypeScript, MIT
Reads a COBOL copybook and decodes mainframe fixed-width records: packed decimal, EBCDIC, implied decimal point, sign in the zone nibble. The kind of thing where a wrong field size does not raise, it just shifts every field after it and returns numbers that look plausible. `REDEFINES` and `OCCURS` refuse with an error on purpose, because accepting them unimplemented would decode silently and return wrong values. 30 tests, CI on Node 20, 22 and 24.

**[wip](https://github.com/daopapp/wip)** &nbsp;·&nbsp; TypeScript, MIT
Tells you what you were in the middle of. Reads the local git state that commit summarisers skip: dirty worktree, conflicted files, stashes, unpushed branches, and the interrupted rebase you forgot about. Sends nothing until the diff has been through redaction, and aborts rather than sending if a credential still looks present at the last gate. 52 tests, including integration tests against real git repositories.

**[software-factory](https://github.com/daopapp/software-factory)** &nbsp;·&nbsp; agents for Claude Code
26 specialised agents (requirements, PO, tech lead, frontend, backend, security, QA, Playwright, devops, DBA, plus one per stack) and a command that dispatches them in parallel waves. Each stack specialist carries the traps of its own technology rather than generic best practice.

---

### What I've been building

Recent product work, under NDA or otherwise private:

- A cross-platform habit and recovery app from a single React and Capacitor codebase, shipped to Android, iOS and web, with subscription billing, three locales, and safety features that route a user in crisis to real support instead of to a chatbot answer
- A developer tool that reads commits from four different Git hosting providers at once and writes the standup summary, with OAuth tokens encrypted at rest under AES-256-GCM and the client locked out of the token collection by security rules
- An internal talent-mapping and task-management portal where assignment is constrained by skill match and remaining capacity, with role-based access enforced in the database rules and covered by 116 tests

---

### How I work

These are my defaults on a project, whether or not anyone asks for them:

- Architecture decisions written as ADRs, so the reasoning outlives the commit
- Security rules covered by their own test suite
- End-to-end tests and accessibility checks running in the pipeline
- Design system in Storybook, with interaction tests
- CI on every push, a preview environment on every pull request
- When I accept a trade-off, I write down what it costs and when to revisit it

---

### Stack

| | |
|---|---|
| **PHP** | Laravel, Symfony, Composer, PSR, REST APIs, JWT, OpenAPI |
| **Front end** | TypeScript, React, Next.js, Vue, Astro, Tailwind, Radix and shadcn/ui, Storybook |
| **Other back end** | Node with Fastify and Express, Python with FastAPI, C# and .NET Core |
| **Mobile** | Capacitor (Android and iOS) |
| **Data** | PostgreSQL, MySQL, MongoDB, Elasticsearch, Redis, Firestore, Oracle and PL/SQL, DB2 |
| **Cloud and infra** | Google Cloud, AWS, Firebase, Docker, GitHub Actions, RabbitMQ, Gearman |
| **AI** | AI agents, RAG, Vertex AI, Claude API and Claude Code |
| **Testing** | Playwright, Vitest, security rules tests, axe |
| **Mainframe** | COBOL, JCL, DB2, CICS, VSAM, TSO |

Portuguese (native), English (B2).

---

### Leading, not only building

Scrum Master on a cross-functional team: ran the ceremonies, removed blockers, owned production incident response with root-cause analysis. Before moving back to hands-on engineering, I spent four years in delivery management at IBM, leading a 23-person team across four baselines totalling around 4,200 hours a month, and before that a development and support team of 22 across core insurance systems. PMI, ITIL and COBIT in practice, not as a certificate.

Industries: telecom, insurance, marketing automation, public sector, and immigration services.

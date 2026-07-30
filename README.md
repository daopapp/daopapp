## Rodrigo Papp

Senior Software Engineer, 16 years. The first half of my career was IBM mainframe (COBOL, DB2, CICS, JCL) in telecom and insurance. The second half has been building and shipping web and mobile products. I use both: the discipline of systems where a bad deploy costs real money, applied to a modern React and Firebase stack.

I take products the whole way: data model, auth, security rules, payments, CI, store release, landing page. Some of it is open source, most of it is not, so the public repository list here is smaller than the contribution graph.

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
| **Front end** | TypeScript, React, Vue, Astro, Tailwind, Radix and shadcn/ui, Storybook |
| **Mobile** | Capacitor (Android and iOS) |
| **Back end** | Node, Firebase (Auth, Firestore, Functions, Hosting), PHP with Laravel and Symfony, C# and .NET |
| **Data** | MySQL, MongoDB, Oracle and PL/SQL, DB2 |
| **Infra** | Docker, GitHub Actions, AWS, Azure, RabbitMQ |
| **Testing** | Playwright, Vitest, security rules tests, axe |
| **Mainframe** | COBOL, DB2, CICS, JCL, VSAM, TSO |

Portuguese (native), English, Spanish.

---

### Before this

Delivery and project management alongside engineering: feasibility analysis, scope and deadline negotiation, cost and quality tracking, following PMI, ITIL and COBIT. Telecom, insurance, marketing, and citizenship and immigration services.

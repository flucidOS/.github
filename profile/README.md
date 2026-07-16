<div align="center">

# FlucidOS

### Computing without chaos.

FlucidOS is an immutable, atomic Linux desktop — engineered so that you can drive your daily work without chaos.

[📂 Documentation](https://drive.google.com/drive/folders/17bUqhZVSesYsYbFdrDtIhNpS4lAcz8fv?usp=sharing) · [Open an Issue](../../issues) · [Meet the Maintainer](https://github.com/siddharthantv)

</div>

---
> [!NOTE]
> Currently we are moving our infrastructure.
> The previous package management method has been discontinued due to architectural and design decision changes
> Soon the infrasture will be shared

## The problem we're solving

Every Linux user knows the feeling. Things are great — until they're not. An update silently breaks something. A config file drifts. A dependency pulls in something unexpected. You spend your Saturday not doing what you sat down to do, but untangling the system underneath it.

Linux doesn't have a power problem. It has a chaos problem.

FlucidOS is our answer to that.

---

## How we solve it

FlucidOS is built on an **immutable, atomic architecture**. The base system is read-only. Updates land as whole-system commits — they either succeed completely, or they don't happen at all. And if a bad update ever makes it through? FlucidOS detects it and rolls back automatically on the next boot.

No manual recovery. No digging through logs at midnight. Just a system that heals itself.

Here's what's under the hood:

| Component | What it does |
|---|---|
| **OSTree** | Atomic system versioning — think Git, but for your entire OS |
| **Flatpak** | Sandboxed, portable app delivery that never touches the base system |
| **Podbx** | Containerised developer environments, fully isolated from the OS |
| **Auto-rollback** | Boot failure after an update? FlucidOS rewinds itself automatically |

The system never drifts. You always know exactly what state you're in. Chaos, by design, has nowhere to live.

---

## Why it exists

> *"The Linux desktop has a user experience problem — not a capability problem."*

FlucidOS exists to close that gap. We're building a desktop that's stable by design, recoverable by default, and genuinely enjoyable to use every day — without hiding the system from people who want to go deeper.

Computing without chaos isn't just a tagline. It's the engineering brief.

---

## Where we are

The foundation is in place and we're building fast:

- Core system developed and documented
- Immutable base and OSTree pipeline are in testing
- Automatic rollback system in testing
- Opening up to contributors — that's where you come in

---

## Come build with us

FlucidOS is opening up, and we genuinely want more people in the room. If you care about Linux, user experience, and systems that are built to last — this is a good place to be.

**Good ways to jump in:**

- **Open an issue** — something feels wrong, missing, or improvable? Tell us, with specifics
- **Propose something** — bring a concrete idea that fits the architecture and explain the why
- **Write code** — clean, purposeful, with a rationale behind every decision

**What doesn't work here:**

- Abstraction for its own sake
- Convenience that trades away system integrity
- Commits without context

We don't have a bar so much as a *style* — thoughtful, deliberate, systems-minded. If that resonates, you'll feel right at home.

---

## What's in scope

| Repository | What lives here |
|---|---|
| Core OS | Base image, OSTree commit pipeline, boot infrastructure |
| Podbx | Container configuration and management |
| Infrastructure | System config, drivers, CI |

---

## Our principles

These aren't rules. They're the values every line of code here is written from:

- **Computing without chaos** — stability and predictability, always
- **Immutability by default** — the base system is never modified at runtime
- **Atomicity over incrementalism** — all or nothing, never halfway
- **User experience first** — power without pain is the whole point
- **Explicit over implicit** — no hidden behavior, no silent defaults

---

## Infrastructure notes

- Development is Git-based
- Repos move fast — stability is explicitly marked when it's guaranteed
- Feedback is always welcome through issues

---

## Disclaimers

FlucidOS is an independent project, not affiliated with any organization, foundation, or distribution. It is not production-ready yet — but it's getting there.

---

<div align="center">

**Maintainer:** [Siddharthan T V](https://github.com/siddharthantv)

*Built correctly first. Now, collaboratively. Come build with us.*

</div>


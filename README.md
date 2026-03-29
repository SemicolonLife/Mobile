# 🧠 System Design Interview Mental Model

**A practical framework for Staff+ engineers who want clarity over complexity in system design interviews.**

---

## 📖 About

Most system design interviews go wrong not because the candidate lacks knowledge — but because they lack **structure**.

This repository contains a battle-tested mental model and reusable prompt/rule file for system design interviews. It helps you:

- **Detect the interview mode** — Frontend, Backend, or Generic
- **Structure your answer** using a proven 15-point framework
- **Avoid the #1 mistake** — going too deep in one area while ignoring everything else
- **Call out tradeoffs** like a Staff+ engineer, not a mid-level candidate

> 📝 **Read the full Medium article:** [Stop Over-Engineering Your System Design Interviews — Use This Mental Model Instead](https://medium.com/@rajanTheSilentCompiler)

---

## 🚀 What's Inside

```
.
├── system-design-mode.mdc      # Cursor IDE rule file (auto-applies to .md/.txt files)
├── system-design-article.md    # Full Medium article in markdown
└── README.md                   # You are here
```

| File | Purpose |
|------|---------|
| `system-design-mode.mdc` | Drop this into your `.cursor/rules/` directory to get AI-assisted system design answers that follow the framework automatically |
| `system-design-article.md` | The complete article explaining the framework — use it as a reference or publish it to your own blog |

---

## 🎯 The 15-Point Framework (Quick Reference)

| # | Section | What to Cover |
|---|---------|---------------|
| 1 | **Problem Statement** | Restate the problem, set scope |
| 2 | **Functional Requirements** | Core user-facing capabilities (4–6 items) |
| 3 | **Non-Functional Requirements** | Latency, availability, consistency, scalability |
| 4 | **End-to-End Flow** | Full workflow from user action → system → result |
| 5 | **Core Components** | 3–5 major building blocks |
| 6 | **API / Interaction Layer** | Key contracts between components |
| 7 | **Data / Storage Choice** | One sensible default DB with rationale |
| 8 | **Client Considerations** | State, rendering, caching, offline behavior |
| 9 | **Scaling** | Horizontal scaling, replicas, CDN |
| 10 | **Caching** | Where it helps, invalidation strategy |
| 11 | **Real-Time / Async** | WebSockets, SSE, queues, workers |
| 12 | **Failure Handling** | Retries, timeouts, idempotency, degradation |
| 13 | **Security** | Auth, encryption, rate limiting |
| 14 | **Tradeoffs / Challenges** | Consistency vs speed, scale spikes, maintainability |
| 15 | **Summary** | Key decisions and the most important tradeoff |

---

## 💡 Three Modes of Operation

The framework adapts based on what the interviewer wants:

### Frontend (FE) Mode
Go heavy on component architecture, state management, rendering strategy, data fetching, client caching, loading/error states, offline behavior, and UX decisions. Keep backend light.

### Backend (BE) Mode
Go heavy on services, APIs, storage, async workflows, scaling, caching, consistency, reliability, and failure handling. Keep client discussion light.

### Generic Mode (Default)
Give a balanced end-to-end design. Cover both client and server at a high level. Focus on the complete workflow. Don't over-index on either side.

> **Pro tip:** If the interviewer doesn't specify, ask: *"Would you like me to focus more on the client-side, the backend, or give a balanced end-to-end design?"* — this alone signals Staff-level maturity.

---

## 🛠️ How to Use

### As a Cursor IDE Rule

1. Copy `system-design-mode.mdc` into your project's `.cursor/rules/` directory
2. It auto-applies to `.md` and `.txt` files
3. Ask your AI assistant to design any system — it will follow the balanced framework automatically

### As an Interview Prep Reference

1. Read through the [Medium article](https://medium.com/@rajanTheSilentCompiler) or `system-design-article.md`
2. Practice 2–3 system design problems using the 15-point structure
3. Use the self-review checklist before wrapping up each practice session

### Self-Review Checklist

Before you say "I think that covers it," verify:

- [ ] Did I describe a complete flow from user action to user result?
- [ ] Did I match the mode the interviewer asked for (FE / BE / Generic)?
- [ ] Did I avoid going too deep in one area at the expense of others?
- [ ] Did I mention failure cases?
- [ ] Did I call out at least two genuine tradeoffs?
- [ ] Did I make a clear, justified database choice?
- [ ] Did I keep capacity estimation reasonable?

---

## 🎯 Who Is This For

- **Staff / Senior / Principal engineers** preparing for system design interviews
- **Mobile platform engineers** transitioning into full-stack or platform-level design rounds
- **Anyone targeting FAANG-tier companies** (Shopify, Stripe, Airbnb, Google, Meta, etc.)
- **Engineering managers** who want a consistent framework for evaluating system design answers

---

## 🤝 Contributing

Found a gap in the framework? Have a better way to handle a specific section? Contributions are welcome.

1. Fork this repo
2. Create a feature branch (`git checkout -b improve-caching-section`)
3. Commit your changes (`git commit -m 'Add distributed caching patterns'`)
4. Push to the branch (`git push origin improve-caching-section`)
5. Open a Pull Request

---

## 📬 Connect

- **Medium:** [@rajanTheSilentCompiler](https://medium.com/@rajanTheSilentCompiler)
- **LinkedIn:** [Rajan Singh](https://www.linkedin.com/in/rajansingh/)
- **GitHub:** [BholuSingh](https://github.com/BholuSingh)

---

## ⭐ Support

If this framework helped you in an interview or your prep, consider giving this repo a star. It helps others find it.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

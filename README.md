# 🏢 AI Office — a full AI company in one Claude skill

Give Claude one goal. A team of **13 AI specialists** takes it from idea to launch: design, code, testing, SEO, video, social media, marketing and sales. A Project Manager coordinates the team and only asks you for decisions.

> **Zero-cost by design:** every role builds on free tiers and open-source tools. The only money you spend is a domain (~$10–15/yr), the Google Play fee ($25 once) and the Apple Developer fee ($99/yr), and only if you need them.

---

## The team

| # | Role | What they deliver |
|---|---|---|
| 1 | 💡 Idea Generator | 5 unique, audience-attracting ideas backed by real evidence, all buildable for free |
| 2 | 🎨 Graphic Designer | Brand guide, SVG logo, app icon, color & font tokens, social media templates |
| 3 | 📐 UI/UX Designer | Personas, user flows, HTML mockups for every screen, component spec |
| 4 | 🖥️ Frontend Programmer | Working web or mobile app (React / Expo / Flutter / PWA) |
| 5 | ⚙️ Backend Programmer | API contract, database, auth and security on free tiers (Supabase, Firebase, Cloudflare) |
| 6 | 🧪 Tester | Real test runs, bug reports, fix loop with programmers, honest verdict |
| 7 | ✅ Validator | Independent judge at two gates: idea scoring and release readiness (store policies, privacy, zero-cost) |
| 8 | 🔍 SEO Specialist | Keywords, on-page & technical SEO, AI-search readiness, App Store Optimization |
| 9 | 🎬 Video Editor | Scripts, storyboards, captions, and rendered short videos when tools allow |
| 10 | 📱 Social Media Handlers | Full post calendars for LinkedIn, Instagram, X, TikTok, Facebook |
| 11 | 📣 Marketing Specialist | Positioning, zero-budget launch plan, content calendar, landing copy, email sequence |
| 12 | 💰 Sales Specialist | Pricing, offers, personalized outreach drafts, objection handling |
| 13 | 📋 Project Manager | Runs the office: brief, task board, handoffs, quality control, reports |

## How it works

```
You: "/ai-office build a habit tracker app for university students and launch it"

Phase 0  Intake         Project Manager writes the brief + task board
Phase 1  Discover       Idea Generator → Validator (Idea Gate)        🔒 you pick the idea
Phase 2  Design         Graphic Designer → UI/UX Designer
Phase 3  Build          Backend (API first) ∥ Frontend → Tester loop
Phase 4  Launch prep    SEO → Validator (Release Gate)                🔒 you approve publishing
Phase 5  Growth         Marketing → Video ∥ Social ∥ Sales            🔒 you approve posts & outreach
Phase 6  Report         Project Manager sends you REPORT.md
```

Everything is saved in `office/<project>/`, so you can stop and resume anytime.

### Safety built in
- **Drafts, not actions.** Nothing is published, posted, sent or paid for without your explicit "approve".
- **No account bans.** No LinkedIn automation, and only official tools for Meta, X and TikTok.
- **Honest output.** Testers must actually run things, and no invented stats or fake reviews are allowed.
- **Anti-spam compliant** sales outreach.

---

## Install

### Claude Code (plugin)
```
/plugin marketplace add <your-github-username>/ai-office
/plugin install ai-office@ai-office
```

### Claude Code (manual)
Copy the skill folder into your skills directory:
```bash
git clone https://github.com/<your-github-username>/ai-office.git
cp -r ai-office/skills/ai-office ~/.claude/skills/
```

### Claude app (claude.ai / desktop)
1. Download this repo and zip the `skills/ai-office` folder (the zip must contain `ai-office/SKILL.md`).
2. Go to **Settings → Capabilities → Skills** and upload the zip.

*(Menu names can change between app versions. If you can't find it, search the Claude help center for "custom skills".)*

---

## Usage

```
/ai-office <your goal>
```

Examples:
- `/ai-office find me a zero-cost app idea for Arabic-speaking freelancers and build the MVP`
- `/ai-office I already have a recipe website — do SEO, social media and a 2-week launch plan`
- `/ai-office just the idea phase: 5 mobile app ideas for gym beginners`

Commands during a project:

| Command | What it does |
|---|---|
| `status` | Shows the task board and what's waiting for you |
| `approve 1, 3` | Approves numbered items from the report |
| `redo <role> <feedback>` | Reruns a role with your feedback |
| `add role <name>` | Adds a new specialist to the team |
| `skip <role>` | Removes a role from this project |

### Keep the office working while you're away
Pair the skill with a scheduled task in Claude, for example:
> "Every weekday at 8am: continue the AI Office project in `office/habit-tracker`, then send me the report."

The team continues where it left off and stops at approval gates, so you only need to say "approve".

---

## Customize

- **Edit a role:** change its file in `skills/ai-office/roles/`.
- **Add a role:** copy any role file, keep the same sections (Mission, Inputs, Process, Output, Quality checklist, Handoff), and add it to the team table in `SKILL.md`.
- **Change the free stack:** edit `skills/ai-office/templates/free-stack.md`.

## Repo structure

```
ai-office/
├── .claude-plugin/
│   ├── plugin.json
│   └── marketplace.json
├── skills/ai-office/
│   ├── SKILL.md              ← the Project Manager's playbook
│   ├── roles/                ← 13 role files
│   └── templates/            ← brief, handoff, report, free stack
├── examples/example-brief.md
├── LICENSE
└── README.md
```

## Honest limits
- AI makes mistakes. Review designs, code and copy before going public; that's what the approval gates are for.
- Running the skill uses your Claude plan's usage. Big projects with all 13 roles use a lot.
- Free tiers change. The team is told to check current limits, but double-check before you scale.
- Some steps need you: creating store and social accounts, filming yourself, and pressing "publish".

## Contributing
PRs welcome: new roles, better prompts, more free tools, translations. Please keep the Zero-Cost Rule and the approval gates.

## License
MIT. See [LICENSE](LICENSE).

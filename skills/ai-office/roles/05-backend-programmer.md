# Role 5 — Backend Programmer

## Mission
Build a secure, simple backend (data, auth, API) that runs entirely on free tiers.

## Inputs
- `00-brief.md`, `03-ux/ux-spec.md`

## Stack choice (free only — see `templates/free-stack.md`)
Prefer **no-server** or **managed free tiers** over running your own server:
- Database + auth: Supabase free tier, Firebase (Spark plan), or Cloudflare D1
- Serverless functions: Cloudflare Workers, Vercel/Netlify functions, Supabase Edge Functions
- If the app can work fully offline/local (localStorage, SQLite on device), that is the cheapest of all — consider it first.

Avoid any service that bills automatically past the free limit without a spending cap. If you must use one, flag it as a risk.

## Process
1. **API contract first.** Write `app/backend/API.md` before coding: every endpoint (or database table + access rule if using Supabase/Firebase directly), request/response shapes, errors, auth requirements. The frontend builds against this.
2. **Data model.** Tables/collections with fields, types, relations. Include a schema/migration file.
3. **Auth.** Use the provider's built-in auth (email magic link, Google sign-in). Never build your own password storage.
4. **Security.** Row-level security / security rules so users can only access their own data. Validate all input. Rate-limit public endpoints where possible. Secrets only in environment variables.
5. **Privacy.** Collect only data the features need. List what's stored in `DATA.md` (the Validator and the privacy policy need it).
6. **Free-tier limits.** Document the limits (requests, storage, rows) and roughly how many users they support.
7. Write basic automated tests for each endpoint/rule. Run them.

## Output — `app/backend/`
- `API.md`, `DATA.md`, schema/migrations, functions code, tests, `README.md` (setup + deploy), `.env.example`
- `app/backend/BUILD-NOTES.md` — choices, limits, risks

## Quality checklist
- [ ] `API.md` written before code and kept in sync
- [ ] Users can't read or change other users' data (tested)
- [ ] Runs on free tiers; limits documented
- [ ] No secrets in code

Finish with the Handoff section → next: **Frontend Programmer** (contract ready) and **Tester**.

# Role 4 — Frontend Programmer

## Mission
Turn the UX spec into a fast, accessible, working interface that talks to the backend API.

## Inputs
- `03-ux/` (spec, mockups, components), `02-brand/tokens.json`, `app/backend/API.md`

## Stack choice (free only — see `templates/free-stack.md`)
- **Web:** HTML/CSS/JS, or React/Vue/Svelte with Vite. Hosting on Cloudflare Pages, Vercel, Netlify or GitHub Pages free tiers.
- **Mobile (Android + iOS from one codebase):** React Native with Expo, or Flutter. A PWA is the cheapest option if the store listing isn't essential.
- Pick the simplest option that meets the brief and explain why in build notes.

## Process
1. Set up the project with a clear folder structure and a `README.md` (install, run, build, deploy).
2. Turn `tokens.json` into theme variables (light + dark).
3. Build reusable components from `components.md` first, then screens.
4. Connect to the API exactly as written in `API.md`. If the backend isn't ready, use a mock layer with the same shapes and note it.
5. Implement every state from the spec (empty, loading, error, offline).
6. Accessibility: semantic HTML / accessible components, labels, focus order, contrast.
7. Performance: lazy-load heavy parts, optimize images, avoid huge libraries.
8. Never put secret keys in frontend code. Use environment variables and only public/anon keys on the client.
9. Run the app and check it actually starts and the core journey works before handing off.

## Output — `app/frontend/`
- Source code, `README.md`, `.env.example`
- `app/frontend/BUILD-NOTES.md` — stack choice, what's done, what's mocked, known limitations

## Quality checklist
- [ ] App runs from a clean install with the README steps
- [ ] Core journey works end to end
- [ ] No secrets committed; `.env.example` present
- [ ] Matches mockups on mobile and desktop

Finish with the Handoff section → next: **Tester**.

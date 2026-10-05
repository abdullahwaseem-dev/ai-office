# Role 8 — SEO Specialist

## Mission
Make the product findable for free: on Google, in AI search engines, and in the app stores.

## Inputs
- `00-brief.md`, `01-ideas.md`, `02-brand/`, `03-ux/`, `app/frontend/`

## Process
1. **Keyword research.** 20–30 keywords grouped by intent (problem-aware, solution-aware, brand). Prefer low-competition long-tail phrases a new site can rank for. Use free tools (Google autocomplete, "People also ask", Google Trends, Search Console once live). Don't invent search volumes; mark estimates as estimates.
2. **On-page SEO (website/landing page).** Title tags, meta descriptions, one H1 per page, heading structure, image alt text, internal links, clean URLs, Open Graph + Twitter card tags.
3. **Technical SEO.** `sitemap.xml`, `robots.txt`, canonical tags, mobile-friendly, fast load, HTTPS, structured data (JSON-LD: `SoftwareApplication`, `Organization`, `FAQPage`).
4. **AI search readiness (GEO/AEO).** Clear FAQ section with direct one-paragraph answers, plain-language "what is X" description, comparison page vs alternatives.
5. **App Store Optimization (if mobile).** App name + subtitle (Apple) / short description (Google), keyword field (Apple, 100 chars), full description, screenshot captions, category choice.
6. **Content plan.** 8–12 blog/article topics targeting the keywords, each with a title, target keyword and outline. Write the first 2 in full.
7. **Free listings.** Product Hunt, relevant directories, Google Search Console + Bing Webmaster setup steps.

Apply the on-page and technical changes directly to the frontend code where possible, and tell the Tester what changed.

## Output — `08-seo.md`
Keyword map, implemented changes list, store listing text, content plan, first 2 articles (or link to files), setup checklist for Search Console.

## Quality checklist
- [ ] Every page has a unique title and description
- [ ] Sitemap, robots and structured data present
- [ ] Store listing text within character limits
- [ ] No keyword stuffing; copy reads naturally

Finish with the Handoff section → next: **Validator (Release Gate)**, then **Marketing Specialist**.

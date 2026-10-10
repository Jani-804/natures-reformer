# Nature Reformer AI Hub — Starter Website

A responsive bilingual (English/Urdu) static homepage starter for the Nature Reformer AI Hub. It includes:
- Home/mission page
- Focus areas: climate, eco-agriculture/IPM, biodiversity, soil and water
- Knowledge-library preview cards
- A clearly labelled **demo** chatbot with example responses
- English/Urdu toggle
- Responsive mobile layout

## Important limitations
- The chatbot is **not connected to a live AI model**. It uses simple example responses in JavaScript.
- Replace the placeholder contact email `hello@naturereformer.org` with an email you control.
- Replace stock image URLs with licensed/owned images before production if desired.
- Add real articles, sources, privacy policy, terms, accessibility checks, and a content review workflow before public launch.
- Do not place any private API key in `index.html`. A live AI connection must call a server-side function/backend that keeps secrets out of the browser.

## Preview locally
Simply open `index.html` in a modern browser. An internet connection is needed for Google Fonts and remote Unsplash photos; the page layout and demo logic are local.

## Low-cost deployment: Cloudflare Pages
1. Create a GitHub repository and upload `index.html` and `README.md`.
2. Sign in to Cloudflare and open Workers & Pages → Create → Pages → Connect to Git.
3. Select the repository.
4. For a plain static site, leave the build command empty and set the output directory to `/` (or the root directory setting shown by the current Cloudflare UI).
5. Deploy and test on phone and desktop.
6. Add a custom domain only after the first version works.

## Recommended next technical steps
1. Create reviewed bilingual knowledge documents with source, date, geography, and reuse permission.
2. Store content metadata in Supabase or another database.
3. Add a server-side API endpoint for the AI model; keep the API key in server-side environment secrets.
4. Implement retrieval-augmented generation (RAG), returning source titles and URLs alongside answers.
5. Add rate limiting, abuse protection, privacy notice, feedback reporting, and a clear disclaimer for high-impact agricultural recommendations.
6. Test a bilingual question set with local agricultural experts before launch.

## Suggested future pages
- `/about` — mission, team, principles
- `/knowledge` — searchable resource library
- `/climate` — climate adaptation and climate literacy
- `/eco-agriculture` — IPM, soil health and pesticide-risk reduction
- `/biodiversity` — pollinators, beneficial insects, wetlands and wildlife
- `/contact` — collaboration and corrections
- `/privacy` and `/terms` — privacy and use terms

This starter currently presents these as homepage sections; separate routes can be added later.

# jonathanwheat.dev

A fast, static Astro website for Jonathan Wheat, independent software developer and technical consultant.

## Run locally

Requires Node.js 20.19+ or 22.12+.

```bash
npm install
npm run dev
```

Open the local URL printed by Astro (usually http://localhost:4321).

## Production build

```bash
npm run build
npm run preview
```

The generated static site is in `dist/`.

## Deploy to Cloudflare Pages

1. Create a GitHub repository under `jwheat`, for example `jonathanwheat.dev`.
2. Push this project's contents to the repository's `main` branch.
3. In Cloudflare, create a **Pages** project using **Import an existing Git repository** (Git integration, not a Direct Upload project).
4. Choose the repository and set framework preset **Astro**, build command `npm run build`, output directory `dist`, and production branch `main`.
5. Deploy. Test the temporary `*.pages.dev` URL.
6. Under the Pages project's **Custom domains**, add `jonathanwheat.dev` and follow Cloudflare's DNS instructions. Add `www.jonathanwheat.dev` if desired, with a redirect to the canonical hostname.

Cloudflare may adjust its UI over time. No environment variables or backend services are required.

## Updating content

- Contact information: `src/components/Footer.astro` and `src/components/Header.astro`
- Intro and statistics: `src/components/Hero.astro`
- Services: `src/components/Services.astro`
- Case studies: `src/components/Projects.astro`
- About and skills: `src/components/About.astro`
- Colors and layout: `src/styles/global.css`
- Downloadable PDF: `public/Jonathan_Wheat_Capabilities.pdf`
- Hero illustration: `public/images/architecture.svg`

## Launch checklist

- [ ] Verify every case study description and contact detail.
- [ ] Confirm GitHub/LinkedIn links and email work.
- [ ] Check layout on phone, tablet, and desktop.
- [ ] Test PDF download and custom domain HTTPS.
- [ ] Review spelling and any personal preferences before sharing widely.

No analytics, cookies, forms, databases, or client-side JavaScript are required.

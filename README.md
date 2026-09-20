# Nustian USA Gala Sponsorship Proposal (site source)

This is the full source of the proposal page. It's a plain static site —
no build step, no framework.

## Run it locally

```bash
npm run dev
```

Then open the URL it prints (usually http://localhost:3000).
(`npm run dev` uses `npx serve`; the first run downloads it automatically.)

No npm? Just open `index.html` directly in a browser — everything works,
including the PDF download button.

## Edit it

- Page content/design: `index.html`
- Logo: `assets/nustian-logo.webp`
- The downloadable proposal PDF: `assets/nustian-usa-sponsorship-proposal.pdf`

The two "Download proposal" buttons are:

```html
<a class="button download"
   href="assets/nustian-usa-sponsorship-proposal.pdf"
   download="nustian-usa-sponsorship-proposal.pdf"
   type="application/pdf"
   aria-label="Download the sponsorship proposal PDF">
```

(There are two of them — one in the header, one in the hero section.)
Swap the `href`/`download` values if you rename the PDF file.

## Deploy

Copy the folder contents to any static host (Netlify, Vercel, GitHub Pages,
Cloudflare Pages, …) — `index.html` + `assets/` is all it needs.

# Get www.byransley.com Live

Your site is one folder: `index.html` + `photos/` (put your hero image in `photos/hero.jpg`).

## Option A: Netlify (easiest)

1. **Sign up:** [netlify.com](https://www.netlify.com) (free account).
2. **Deploy:** Drag and drop your **project folder** (the one that contains `index.html` and `photos`) onto the Netlify dashboard. Your site gets a URL like `random-name.netlify.app`.
3. **Add your domain:** In Netlify: **Site settings → Domain management → Add custom domain**. Enter `www.byransley.com`.
4. **DNS (where your domain is managed):** Add the records Netlify shows you, usually:
   - **CNAME** for `www` → `random-name.netlify.app` (or the hostname Netlify gives you).
   - For the root `byransley.com`, Netlify may give you an A record or recommend their DNS; follow their instructions.
5. **HTTPS:** Netlify will issue a free SSL certificate once DNS is pointing to them (can take a few minutes to 48 hours).

Done. Visit **https://www.byransley.com** and it should load.

---

## Option B: Vercel

1. Sign up at [vercel.com](https://vercel.com).
2. **Import:** New Project → upload or connect the folder with `index.html`.
3. **Add domain:** Project → Settings → Domains → add `www.byransley.com`.
4. In your domain DNS, add the CNAME record Vercel shows you for `www`.

---

## Your domain (Google Workspace / Squarespace Domains)

- Where you **manage DNS** (Google Domains, Squarespace Domains, or whoever hosts byransley.com): add the **CNAME** and/or **A** record your host (Netlify/Vercel) tells you.
- Keep your **MX records** as they are so email (you@byransley.com) keeps working.

---

## After it’s live

1. Put **hero.jpg** in the `photos/` folder and re-upload so your face shows and link previews use it.
2. **Google Search Console:** [search.google.com/search-console](https://search.google.com/search-console) → Add property → `https://www.byransley.com`. Submit the sitemap if you add one later (optional for a single page).
3. Share the link; Open Graph will use `photos/hero.jpg` for previews.

# Best Property Management Tools — Site Files

Plain static site: `index.html`, `styles.css`, `script.js`. No build step, no dependencies.

## Deploy to Vercel (free) — two options

### Option A: Drag and drop (fastest, no GitHub needed)
1. Go to https://vercel.com and sign up / log in (free tier is fine).
2. Click "Add New" → "Project."
3. Choose "Deploy" via the drag-and-drop upload option (Vercel supports uploading a folder directly for static sites).
4. Drag this whole folder in.
5. Once deployed, go to Project Settings → Domains → add `bestpropertymanagementtools.com`.
6. Vercel will give you DNS records (usually an A record and/or CNAME) to add at Namecheap:
   - Log into Namecheap → Domain List → Manage → Advanced DNS
   - Add the records Vercel shows you
   - DNS propagation can take a few minutes to a few hours

### Option B: GitHub (better long-term — makes future edits easier)
1. Create a free GitHub account if you don't have one.
2. Create a new repository, e.g. `bpmt-site`.
3. Upload these three files (`index.html`, `styles.css`, `script.js`) to it.
4. In Vercel, "Add New" → "Project" → "Import Git Repository" → select the repo.
5. Leave build settings blank/default (static site, no framework) → Deploy.
6. Connect the custom domain the same way as Option A, step 5-6.

## Editing content later
Everything is in `index.html` — no templating engine, just look for the section you want to change (each is commented, e.g. `<!-- DIRECTORY BOARD -->`). Prices and copy are plain text in the HTML.

## Next steps once live
- Replace the `#` placeholder links in the directory board and comparison table with your real affiliate tracking links once Buildium/DoorLoop/AppFolio approve you.
- Add the Affiliate Disclosure and Privacy Policy pages (linked in the footer, currently placeholders).
- Add Google Analytics / Search Console verification tags to the `<head>` in `index.html`.

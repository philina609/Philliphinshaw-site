v6 — Browser Editor Enabled (Decap/Netlify CMS)
===============================================
This bundle includes a web-based admin at /admin so you can edit text/links without zipping/redeploying manually.

How it works
- All editable content lives in /content/data.json
- The homepage fetches that JSON and renders it
- /admin (Decap CMS) lets you edit the JSON in a nice GUI
- On Netlify with Git Gateway, your edits auto-commit to your repo → redeploys happen automatically

Setup (one-time)
1) Create a GitHub repo and push these files.
2) In Netlify, create a site from that repo.
3) In Netlify → Site settings → Identity:
   - Enable Identity
   - Enable "Git Gateway"
   - Invite yourself (your email) as a user
4) Open https://YOURDOMAIN/admin/ and log in. Edit content visually and click "Publish".

Daily use
- Visit /admin to change titles, cards, descriptions, links, disc bag, etc.
- Save/Publish → Netlify auto-builds and updates the live site.

Notes
- If you prefer Cloudflare Pages, you can switch the CMS backend to "github" and log in via GitHub directly.

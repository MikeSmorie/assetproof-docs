# AssetProof — how my edits reach the public

**The key idea:** I edit the *master* files in your Dropbox. The public never sees Dropbox — they see *copies* hosted in three places. A change only goes live when its copy is placed. Nothing publishes itself.

## The three destinations

1. **GitHub repo `assetproof-docs`** — your "file cabinet on the web" (GitHub Pages). Hosts all your static files **and the concierge's brain**: the guide HTML, the PDFs, the preview image, and the concierge `.md` files. Your action: on github.com, drag the file in (replacing the old one) and commit. *The live concierge reads its brain from here* — so replacing `concierge-system.md` updates the bot on its very next reply, no redeploy.

2. **Hostinger Horizons** — your website, assetproofsolutions.com. Your action: paste the prompt → review → **Publish**.

3. **Replit** — the concierge *app* itself (code, secrets, database). Your action: paste a prompt into the Replit agent, or set a secret. (Its words come from GitHub; its plumbing lives here.)

## This batch — what to do now

All GitHub files are staged together in: `AssetProof — Guest Guides (giveaway)/Cape Town/_Upload to GitHub (assetproof-docs)/`

| What changed | Goes live via | Your action |
|---|---|---|
| Guide social thumbnail (`guide-preview.png`) | GitHub | upload to `assetproof-docs` |
| Guide page — concierge buttons + social meta + global line (`cape-town-guide.html`) | GitHub | upload (replace) |
| Full guide, one-pager, host one-pager (3 PDFs) | GitHub | upload |
| **Concierge brain — global thread** (`concierge-system.md`) | GitHub | upload (replace) → bot self-updates |
| Concierge Cape Town pack (`concierge-cape-town.md`) | GitHub | upload (replace) |
| Website "Free Guest Guide" host section | Horizons | paste `HORIZONS PROMPT — Host Guest-Guide section.md` → Publish |
| Sign-up "something went wrong" | Replit | paste the database prompt from the earlier message |

**After uploading the guide HTML:** run its public link once through Facebook's Sharing Debugger to refresh the preview, then it's fully live — connected concierge and all.

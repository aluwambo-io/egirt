# eGIRT: eGovernance in Real Time

Low-fidelity prototype of a real-time, multilingual e-participation platform for Uganda.
Static site: `index.html` is the whole app (no build step).

## Deploy to Vercel

### Option A: GitHub (recommended)
1. `git init && git add . && git commit -m "eGIRT prototype"`
2. Create a GitHub repository and push.
3. On vercel.com choose Add New > Project, import the repo, keep Framework Preset = Other, click Deploy.
4. Every later `git push` redeploys; pull requests get preview URLs.

### Option B: CLI
```
npm i -g vercel
vercel        # accept defaults
vercel --prod
```

## Run locally
Open `index.html` in a browser, or run `npx serve .`

## Next steps
- Add `/api` serverless functions and a database (data currently resets on reload)
- OTP phone verification; store only a salted hash of the number
- Real USSD via a gateway such as Africa's Talking
- Embedding-based duplicate detection; machine translation of issue text
- Pseudonyms instead of last three digits on public reports

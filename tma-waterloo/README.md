# TMA UW-WLU — Landing Page

## 🚀 Deploy to Vercel (thaqalaynma.ca)

### Option 1: Vercel CLI (Fastest)
```bash
npm install -g vercel
cd tma-waterloo
vercel --prod
```
Then in your Vercel dashboard → Project Settings → Domains → Add `thaqalaynma.ca`

### Option 2: Vercel Dashboard (No CLI)
1. Push this folder to a GitHub repo
2. Go to [vercel.com](https://vercel.com) → New Project → Import your repo
3. Framework Preset: **Other** (no build step needed — it's pure HTML)
4. Click Deploy
5. Go to Settings → Domains → Add `thaqalaynma.ca`

### Option 3: Drag & Drop
1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag and drop this entire `tma-waterloo` folder
3. Add your custom domain in project settings

---

## 📁 File Structure
```
tma-waterloo/
├── index.html       # Main landing page
├── style.css        # All styles
├── main.js          # Interactions & animations
├── vercel.json      # Vercel routing config
├── public/
│   └── logo.png     # TMA logo (white text)
└── README.md        # This file
```

## 🔗 Custom Domain Setup
After deploying, point your domain DNS:
- Add a CNAME record: `thaqalaynma.ca` → `cname.vercel-dns.com`
- Or use Vercel's nameservers for automatic SSL

## ✏️ Updating Content
- **Events**: Edit the `.event-card` blocks in `index.html`
- **Social links**: Update `href` attributes in the Connect section
- **Stats**: The counters auto-animate from `main.js` — update the `targets` array
- **Term label**: Change "Winter 2026 Term" in the hero badge

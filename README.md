# REK Therapy Website — Deployment Guide
## rektherapy.com · Tracy Croghan, LICSW

---

## What's in this folder

```
rektherapy/
├── index.html        ← Your complete website
├── api/
│   └── claude.js     ← Secure API function (hides your API key)
├── vercel.json       ← Vercel configuration
└── README.md         ← This guide
```

---

## Step 1 — Get your Claude API Key (5 min)

1. Go to https://console.anthropic.com
2. Sign up with your email
3. Click **API Keys** in the left menu
4. Click **Create Key** — name it "REK Therapy"
5. **Copy the key immediately** — you won't see it again
6. Save it somewhere safe (like a password manager)

---

## Step 2 — Create a Vercel Account (2 min)

1. Go to https://vercel.com
2. Click **Sign Up** — use Google or email
3. Complete the quick onboarding (choose "hobby" / free plan)

---

## Step 3 — Deploy the Website (5 min)

### Option A: Drag & Drop (Easiest)
1. Go to https://vercel.com/new
2. Click **"Upload"** or drag the entire `rektherapy` folder onto the page
3. Click **Deploy**
4. Vercel gives you a live URL like `rektherapy.vercel.app`

### Option B: Via GitHub (Recommended for updates)
1. Create a free account at https://github.com
2. Create a new repository called `rektherapy`
3. Upload all files from this folder
4. In Vercel, click **"Import Git Repository"** and connect your GitHub
5. Select the `rektherapy` repo and click **Deploy**

---

## Step 4 — Add Your API Key (2 min) ⚠️ IMPORTANT

This is what makes the AI features work securely.

1. In your Vercel dashboard, click your project
2. Go to **Settings → Environment Variables**
3. Click **Add New**
4. Name: `ANTHROPIC_API_KEY`
5. Value: paste your Claude API key
6. Click **Save**
7. Go to **Deployments** and click **Redeploy**

Your API key is now securely stored — it never appears in your website code.

---

## Step 5 — Buy Your Domain (10 min)

1. Go to https://namecheap.com
2. Search for `rektherapy.com`
3. Purchase it (~$12/year)

---

## Step 6 — Connect Your Domain to Vercel (5 min)

1. In your Vercel project, go to **Settings → Domains**
2. Type `rektherapy.com` and click **Add**
3. Vercel shows you two DNS records to add
4. Log into Namecheap → Manage your domain → Advanced DNS
5. Add the records Vercel gives you
6. Wait 10-30 minutes for the domain to go live

---

## Step 7 — Customize Your Content

Open `index.html` and search for these placeholders to update:

- `(402) 555-0100` → your real phone number
- `hello@rektherapy.com` → your real email
- `$150/session` → your actual rate
- `TC` initials block → replace with a real photo (add `<img>` tag)
- Office hours → update to your real availability

---

## Total Cost Summary

| Item | Cost |
|------|------|
| Vercel hosting | Free |
| rektherapy.com domain | ~$12/year |
| Claude API (AI features) | ~$1-3/month |
| **Total** | **~$27 first year** |

---

## Need Help?

- Vercel docs: https://vercel.com/docs
- Anthropic API: https://docs.anthropic.com
- Domain setup: https://www.namecheap.com/support/

---

*Built with Claude AI · REK Therapy · 2026*

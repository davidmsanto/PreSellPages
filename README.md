# PreSellPages — PickOrAChoice

High-converting, compliant presell landing page for the **BuzzFarmsAI Live Online Workshop** on `https://pickorachoice.com/buzzfarmsai`.

## Structure

```
PreSellPages/
├── index.html              # Main landing page (root level)
├── buzzfarmsai/
│   └── index.html          # Subfolder landing page (for https://pickorachoice.com/buzzfarmsai)
├── .gitignore
└── README.md
```

## Hostinger Deployment Guide

1. Log in to **Hostinger hPanel**.
2. Go to **Websites** &rarr; Select `pickorachoice.com` &rarr; **Manage**.
3. Under **Advanced**, click on **Git**.
4. Configure Git Repository:
   - **Repository**: `https://github.com/davidmsanto/PreSellPages.git`
   - **Branch**: `main`
   - **Install Path**:
     - Option A (Full site): `public_html` (serves `pickorachoice.com` and `pickorachoice.com/buzzfarmsai/`)
     - Option B (Subdirectory only): `public_html/buzzfarmsai`
5. Click **Create** / **Deploy**.
6. (Optional Auto-Deploy Webhook): Copy the Webhook URL provided by Hostinger and paste it into GitHub:
   - Go to `https://github.com/davidmsanto/PreSellPages/settings/hooks`
   - Click **Add webhook**
   - Payload URL: Paste the Hostinger Webhook URL
   - Content type: `application/json`
   - Click **Add webhook**

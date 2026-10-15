# Moving the calculator to Vercel (later)

The repo is already Vercel-ready: `index.html` sits at the root, with no build step.

## 1. Import the repo into Vercel
1. Log in to Vercel. Click **Add New** > **Project**.
2. Pick the GitHub repo `va-calculator` and click **Import**.
3. Framework Preset: **Other**.
4. Leave **Build Command** and **Output Directory** empty.
5. Click **Deploy**. Vercel gives you a `*.vercel.app` URL. Check it loads.

## 2. Add your custom domain
1. In the Vercel project, open **Settings** > **Domains**. Add your domain.
2. Vercel shows DNS records (usually an A record and/or a CNAME). Add those at your domain registrar.
3. Wait for Vercel to show the domain as verified. DNS can take minutes to a day.

## 3. IMPORTANT: do this BEFORE pointing the domain at Vercel
GitHub Pages and Vercel will fight over the same domain if both claim it.
1. In GitHub: repo **Settings** > **Pages** > **Custom domain**. If anything is there, clear it and save.
2. In the repo: if a file named `CNAME` exists at the root, delete it and push.
Only then add the DNS records from step 2.

## 4. After Vercel is live
Decide whether to turn GitHub Pages off (repo **Settings** > **Pages** > Source: **None**).
A repo can stay connected to both. Leaving Pages on keeps the `github.io` URL working as a backup; turning it off avoids two copies of the site.

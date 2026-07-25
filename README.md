# Smart Steps Montessori — Website

A modern, responsive rebuild of the Smart Steps Montessori website
(smartstepsmontessori.com), ready to deploy on GitHub Pages.

## What's in here

Plain HTML + CSS + a small bit of vanilla JS — no build step, no
framework, no dependencies to install.

```
index.html            Introduction (homepage)
our-montessori.html    Our Montessori + family reviews
philosophy.html        Philosophy
tuition.html           Tuition
summer-program.html    Super Summer Program
calendar.html          Calendar
our-day.html           Our Day (daily schedule)
for-parents.html       For Parents
careers.html           Careers
contact.html           Contact Us + map
404.html               Not-found page
assets/css/style.css   All styling
assets/js/main.js      Mobile menu toggle
assets/images/         Photos and logo
```

## Deploying to GitHub Pages

1. Create a new repository on GitHub (or use an existing one).
2. Upload every file in this folder to the root of that repository,
   keeping the `assets` folder structure intact. The easiest way:
   drag-and-drop everything into the GitHub web UI, or:

   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```

3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to `Deploy from a
   branch`, choose the `main` branch and the `/ (root)` folder, then
   click **Save**.
5. GitHub will give you a URL like
   `https://<your-username>.github.io/<your-repo>/` within a minute
   or two — that's your live site.

### Using a custom domain (optional)

If you want `smartstepsmontessori.com` to point at this instead of
the old host:

1. In **Settings → Pages**, enter the domain under **Custom domain**
   — this creates a `CNAME` file in your repo automatically.
2. At your domain registrar, point the domain's DNS to GitHub Pages
   (an `A` record set for apex domains, or a `CNAME` record for a
   `www` subdomain — GitHub's Pages settings page shows the exact
   values to use once you type in your domain).

## Updating content later

Everything is plain HTML, so text edits are just editing the
relevant `.html` file in a text editor and pushing the change —
no rebuild needed. All nine pages share the same header, footer,
and `assets/css/style.css`, so a style change in that one file
updates the whole site.

## Notes

- The **Calendar** page intentionally doesn't hard-code this
  school year's dates (the old site's calendar graphic was tied to
  a specific year and would go stale) — swap in your current
  calendar whenever you'd like, either as text or as a downloadable
  image/PDF linked from that page.
- The **Careers** page uses the email address from the original
  site's careers page; the **Contact** page uses the Gmail address
  from the original contact page. Double check both still route
  where you want.
- The Google Map embed and Calendly tour link were carried over
  from the original site as-is.

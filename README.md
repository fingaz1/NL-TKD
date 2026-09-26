# nl-tkd.com — No Limits Taekwondo

Static site for GitHub Pages. No build step needed; edit the HTML files directly.

## Files
- index.html, about.html, classes.html, forms.html, contact.html
- blog/index.html (post list) and blog/master-william.html (the Oct 2023 post)
- 10-hand-blocking-video.html redirects to forms.html#ten-hand
- style.css (all styling), assets/ (logo, favicon, photos)
- CNAME (tells GitHub Pages the custom domain), 404.html

## Deploy
1. Create a repo (e.g. `nl-tkd`), push these files to `main`.
2. Repo Settings > Pages > Source: Deploy from a branch > `main` / root.
3. Custom domain: `nl-tkd.com` (CNAME file already included). Tick "Enforce HTTPS" once it's available.
4. At the domain registrar, remove the current forwarding/frame setup and add:
   - A records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - CNAME for `www`: `<your-github-username>.github.io`
5. After DNS switches over, cancel/unpublish the Wix site.

## Common edits
- Add a blog post: copy blog/master-william.html, change the text, add a card to blog/index.html.
- Add a form video: copy one `<li class="form">` block in forms.html and swap the YouTube ID (in both the data-id and the thumbnail URL).
- Contact form: see the commented Formspree block in contact.html.

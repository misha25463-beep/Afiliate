# Affiliate.top landing page

Static one-page website prepared for GitHub Pages and a custom domain.

## Files

- `index.html` - page content
- `styles.css` - layout, responsive styles and palette
- `script.js` - mobile navigation and reveal animations
- `assets/affiliate-top-logo.png` - provided Affiliate.top logo
- `assets/product-visual.svg` - custom hero illustration
- `assets/favicon.svg` - browser icon
- `CNAME.example` - custom-domain template

## Publish with GitHub Pages

1. Create a GitHub repository.
2. Upload all files from this folder to the repository root.
3. Open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder.
6. Save and wait for GitHub Pages to publish the site.

## Connect a custom domain

1. In **Settings > Pages**, enter your domain under **Custom domain**.
2. Add the DNS records GitHub shows for your setup at your domain provider.
3. Turn on **Enforce HTTPS** after DNS verification completes.

A `CNAME` file will be created automatically by GitHub when the custom domain is saved in Pages settings. You can also add it manually with only the domain name inside.

## Google Play link

The Google Play button currently shows **In development** and intentionally points to the page section itself.

After the Android app is published, replace this in `index.html`:

```html
href="#google-play" aria-disabled="true"
```

with the real Google Play URL and remove `aria-disabled="true"`. You can also change the button text from `In development` to `Get it on Google Play`.

## Local preview

Run from the project folder:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

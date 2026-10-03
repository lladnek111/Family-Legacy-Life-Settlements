# Family Legacy Life Settlements — website

A single-page website for Family Legacy Life Settlements, an independent life settlement broker based in Kaysville, Utah. No build step: plain HTML, CSS and JavaScript.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site: every page, styles and scripts |
| `hero-couple.jpg` | Homepage hero photo |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `family-legacy-site`).
2. Upload these files to the repository root (Add file → Upload files), then commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Use your own domain (optional)

1. Buy a domain (for example from Namecheap, Squarespace or Cloudflare).
2. In **Settings → Pages → Custom domain**, enter it and save. GitHub adds a `CNAME` file.
3. At your domain registrar, add the DNS records GitHub shows you, then turn on **Enforce HTTPS** once it is available.
4. Update `https://www.[your-domain].com` in the two schema blocks near the top of `index.html`.

## Make the forms send to you

The evaluation, contact and professional forms validate and show a thank-you screen, but they send nothing until you connect a form service. GitHub Pages cannot receive form submissions by itself.

1. Create a form at a service such as Formspree (free tier available). It gives you an endpoint like `https://formspree.io/f/abcdwxyz`.
2. In `index.html`, search for `const FORM_ENDPOINT=""` and paste the endpoint between the quotes.
3. Commit. Submissions now arrive in the service's inbox and your email. Each one includes a `form` field naming which form it came from.

Choose a service whose privacy terms fit the information you collect (age, policy details, general health). Have counsel confirm before launch.

## Before launch

- Have an elder law attorney review the Medicaid & Planning page and the Medicaid FAQ answers.
- Have counsel review the Privacy Policy, form consent language and how submissions are stored. Confirm Section 8 of the policy is accurate.
- Confirm the professional network the site describes is in place.
- Add an email address, office location or hours when you have them.
- Add licensing for any other state before serving clients there.
- Replace placeholder photography on inner pages if you add more images.

## Editing tips

- Page text lives directly in `index.html`. Search for the sentence you want to change.
- Repeated content (FAQ, examples, process steps, qualification cards, professional network) is stored in JavaScript lists near the bottom of the file (`FAQ`, `EXAMPLES`, `PROCESS`, `QUALIFY`, `NETWORK`). Edit the list and every place it appears updates.
- Colors and fonts are defined once at the top of the `<style>` block.

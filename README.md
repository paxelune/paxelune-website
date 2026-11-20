# PAXELUNE Official Website

Static website for PAXELUNE and its first product, PAXELUNE LIFE.

## Files
- `index.html` — homepage
- `support.html` — support and FAQ
- `privacy-policy.html` — public privacy policy
- `terms.html` — terms of service
- `delete-account.html` — account deletion instructions and email request helper
- `assets/` — official logos and visual assets
- `css/style.css` — styles
- `js/main.js` — navigation, FAQ, and form interactions

## GitHub Pages deployment
1. Create a GitHub repository, for example `paxelune-website`.
2. Upload the entire contents of this folder to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to publish the website.

## Configure Google Play link
Open `js/main.js` and set:
`const playStoreUrl = 'https://play.google.com/store/apps/details?id=YOUR_REAL_PACKAGE_ID';`
Use the actual published Google Play URL only. Until then, buttons show a Coming Soon state.

## Account deletion
The static account deletion form prepares an email to `paxelune@gmail.com`; it does not submit or process a deletion automatically. Before publishing the page URL in Google Play Console, ensure the support mailbox is monitored and the developer has a working process to verify requests and delete associated account/cloud data. If an automated endpoint is implemented later, connect it securely and update the page to accurately describe its behavior.

## Important pre-publication checks
- Verify the Privacy Policy against the production app, Firebase setup, SDK data practices, and Google Play Data Safety form.
- Verify that the in-app Delete Account & Data action deletes the intended local and cloud records.
- Test the external account deletion request process end-to-end.
- Add the real Play Store listing URL.
- Test all pages on mobile and desktop.
- If using a custom domain, configure it in GitHub Pages and enforce HTTPS.

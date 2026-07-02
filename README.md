# Whiskay — Privacy Policies

Static site hosting privacy policies for Whiskay apps, served via GitHub Pages.

**Live site:** https://whiskay.github.io/privacy-policy/

## Structure

```
index.html              Home page listing all app policies
assets/style.css        Shared stylesheet for all pages
<app-slug>/index.html   One folder per app; the folder name is the permanent URL slug
.nojekyll               Disables Jekyll so files are served as-is
```

## URLs

| Page        | URL                                                    |
| ----------- | ------------------------------------------------------ |
| Home        | https://whiskay.github.io/privacy-policy/              |
| Tic Tac Toe | https://whiskay.github.io/privacy-policy/tic-tac-toe/  |

Use the **app-specific URL** in Google Play Console (App content → Privacy policy),
not the home page.

## Adding a new app

1. Copy an existing app folder, e.g. `cp -r tic-tac-toe/ new-app-slug/`
2. Edit `new-app-slug/index.html`: app name, date, and the data-collection
   sections to match what the app actually does (keep or delete the
   Third-Party Services block accordingly).
3. Add a card for it in `index.html` on the home page.
4. Commit and push. The policy is live at
   `https://whiskay.github.io/privacy-policy/new-app-slug/` within a minute or two.

## Rules

- Never rename an app folder after its URL has been submitted to a store.
- Keep the policy text consistent with the app's Play Console Data Safety form.
- Update the "Last updated" date whenever the policy text changes.

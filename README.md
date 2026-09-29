# Family Rights: Privacy Policy

The public privacy policy for the Family Rights Android app, served with GitHub Pages.

- **Policy URL:** https://gooderman932.github.io/family-rights-privacy/
- **Account deletion URL (Play Console → Data safety):** https://gooderman932.github.io/family-rights-privacy/#delete

## Before publishing

`index.html` contains two tokens you must replace: `{{OPERATOR_NAME}}` (the legal entity shown as the developer on
Google Play) and `{{CONTACT_EMAIL}}` (a monitored privacy/support inbox). Then check that the policy matches your
Play Console **Data safety** answers. Google rejects listings where the two disagree.

```bash
sed -i 's/{{OPERATOR_NAME}}/Your Company LLC/g; s/{{CONTACT_EMAIL}}/privacy@example.com/g' index.html
grep -n '{{' index.html || echo "No placeholders left"
```

## Enabling GitHub Pages

Repository **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.

## Updating the policy

Edit `index.html` and change the "Last updated" date. For material changes, notify users in the app before they take effect.

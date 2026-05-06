# sellforme-oauth

Static bridge pages for SellForMe's eBay OAuth flow.

The iOS app uses `ASWebAuthenticationSession` with the custom URL scheme `sellforme://`, but eBay only redirects to HTTPS URLs. These pages catch eBay's redirect and forward the query string to the app's custom scheme.

## Pages

- `privacy.html` — Privacy Policy URL
- `callback.html` — Auth Accepted URL → forwards to `sellforme://callback?...`
- `declined.html` — Auth Declined URL → forwards to `sellforme://declined?...`

Hosted via GitHub Pages.

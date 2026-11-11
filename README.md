# boxbuddy.net

Static website for the BoxBuddy iOS app: landing page, support, privacy policy and terms.
Plain HTML/CSS, with no build step. Every page is a folder with an `index.html`, so URLs stay clean on any host.

| URL | File | Used by |
|---|---|---|
| https://boxbuddy.net/ | `index.html` | App Store marketing URL |
| https://boxbuddy.net/support/ | `support/index.html` | App Store Connect support URL |
| https://boxbuddy.net/privacy/ | `privacy/index.html` | `APIConfig.privacyURL`, App Store Connect, Google OAuth consent screen |
| https://boxbuddy.net/terms/ | `terms/index.html` | `APIConfig.termsURL`, subscription Terms of Use |

The privacy policy here is the published copy. Keep it in sync with the app repo's `docs/privacy-policy.md`
and `BoxBuddy/PrivacyInfo.xcprivacy` whenever the data the app collects changes.

The header and footer are repeated in each page. Change them in every file.

Preview locally: `python3 -m http.server 8080`, then open http://localhost:8080.

`CNAME` sets the custom domain for GitHub Pages. Other hosts ignore it.

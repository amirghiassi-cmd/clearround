ClearRound website — updated 6 September 2026

Open index.html in a browser to preview it.

This version includes:
- Updated positioning for sole-trader / one-round window cleaners
- £29.99/year unlimited pricing (free up to 25 active customers retained)
- iPhone and iPad support messaging
- CSV import and export explanations
- iCloud backup explanation
- Stripe / Tap to Pay explanation and fee disclaimer
- New screenshot gallery using the supplied ClearRound screenshots
- High-level comparison with Squeegee, CleanerPlanner and Aworka
- Updated FAQ and pricing sections

Competitor pricing/features used in the comparison were checked on 6 September 2026 and should be reviewed periodically because competitor plans can change.

Before publishing:
1. Change mail@clearroundapp.com to your real support email.
2. Privacy Policy is now included as privacy.html and linked from the website footer.
3. Replace the 'App Store — Coming Soon' button with your App Store URL when live.
4. If your Stripe implementation does not support Tap to Pay, remove that sentence from the Stripe feature card.

Free hosting options:
- GitHub Pages
- Cloudflare Pages
- Netlify

Privacy page added 6 September 2026. Before publishing, replace mail@clearroundapp.com in both index.html and privacy.html with your real support/privacy email address.
STRIPE CONNECT AND UNIVERSAL LINKS
----------------------------------
This package includes:

- /stripe/return/ — fallback page after Stripe Connect onboarding
- /stripe/refresh/ — fallback page for expired onboarding links
- /.well-known/apple-app-site-association — Apple Universal Link association
- /apple-app-site-association — root fallback copy for Apple
- /.nojekyll — ensures GitHub Pages publishes the .well-known directory

The association file authorises:
J667L5G36E.com.amirghiassi.ClearRoundApp

In Xcode, the ClearRound app target must include this Associated Domain:
applinks:clearroundapp.com

After uploading, verify that these addresses load without a redirect:
https://clearroundapp.com/.well-known/apple-app-site-association
https://clearroundapp.com/stripe/return/
https://clearroundapp.com/stripe/refresh/

The apple-app-site-association response should be served over HTTPS and should
not return an HTML error page. The file deliberately has no .json extension.

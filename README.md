# simonschubert.github.io

The root of simonschubert.github.io. The projects live in their own repos, at
their own paths (`/omarchy-widgets/` is the widget store).

`.well-known/assetlinks.json` lets Omalauncher open widget share links
(`https://simonschubert.github.io/omarchy-widgets/w#owl1.…`) straight from the
camera, instead of the browser. Android reads it from the domain's root, which
is why it is here and not in the store's repo. It lists every key the app is
signed with:

- the debug key builds from this machine use
- the upload key, for release builds installed without Play
- the Play app signing key (Play Console → App integrity → App signing), for
  installs from Google Play

`.nojekyll` keeps GitHub Pages from dropping `.well-known`, which Jekyll would
skip as a hidden folder.

# officezied-prog.github.io

Root site of the Khair Mart apps (the apps themselves live in `officezied-prog/zied` under `/zied/khair-pos/`).

- `index.html` sends visitors to the install page: https://officezied-prog.github.io/zied/khair-pos/install.html
- `.well-known/assetlinks.json` (Digital Asset Links) proves that the Khair Mart Android apps
  (`com.khairmart.owner`, `com.khairmart.kasir`, `com.khairmart.sales`, `com.khairmart.gudang`) belong to this site,
  so Android opens them full screen without an address bar. It must hold the SHA-256 fingerprint of the signing key that
  `officezied-prog/zied` → `.github/workflows/android.yml` creates (committed there as `khair-pos/android/assetlinks.json`).
- `.nojekyll` makes GitHub Pages serve the `.well-known` folder as it is.

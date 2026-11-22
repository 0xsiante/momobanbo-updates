# momobanbo-updates

Signed update files for the MoMoBanbɔ Android app. **No source code, SMS data or keys are kept here.**

- `protection/manifest.json` lists each file with its SHA-256 and size, plus a version number.
- `protection/manifest.json.sig` is an ECDSA P-256 / SHA-256 signature of the manifest. The private key is offline.
- The app installs a set only if the signature matches the public key built into the app, the version is newer than the installed one, and every file matches its hash. Otherwise it keeps what it has.

The app only downloads from here (HTTPS GET). It never uploads anything.

# AI Quote Pro — downloads

Public download host for the **AI Quote Pro** Android app. This repository
holds no source code; it exists only so the release binaries have a stable,
publicly reachable URL. The application itself is developed in a private
repository.

## Get the app

Download the latest APK from the [Releases page](https://github.com/Muskzw/AIquote-releases/releases/latest).

Android 7.0 or later. Because the app is installed directly rather than
through the Play Store, Android will ask you to allow installation from
unknown sources the first time.

## Verifying a download

Every release lists the APK's SHA-256 alongside the signing certificate
fingerprint. The two answer different questions: the SHA-256 tells you the
file downloaded intact, and the certificate tells you it was built and signed
by us.

Check the file you downloaded:

```bash
sha256sum AIQuotePro-v1.1.1.apk
```

Check who signed it, if you have the Android build tools:

```bash
apksigner verify --print-certs AIQuotePro-v1.1.1.apk
```

Every release from v1.0.0 onward is signed with the same key, so each new
version installs over the previous one without uninstalling and without
losing any of your data:

```
CN=AI Quotation Maker, OU=Mobile, O=techub, L=Harare, ST=Harare, C=ZW
SHA-1  84:1A:15:74:25:02:7C:4D:02:37:C7:DD:CD:22:2A:00:1E:B2:52:9B
```

If an APK you find elsewhere reports a different fingerprint, it was not
signed by us — do not install it.

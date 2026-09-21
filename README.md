# SomeHowTosAndTexts

The static-file bucket for my apps. It holds the JSON and HTML that my Android apps fetch at runtime over `raw.githubusercontent.com` — so I can update them without shipping an app update, and host them for free.

Not a project you run — a place things are served from.

## What's in here

| Kind | Count | What it's for |
|---|---|---|
| `privacy_policy.html` / `terms_and_conditions.html` | ~20 | The privacy policies and terms each app links to (Play Store requires a hosted URL) |
| `updater.json` | ~12 | Version-check payloads read by [AndroidAppUpdater](https://github.com/p32929/AndroidAppUpdater) — bump the version here to prompt an in-app update |
| `HouseAdsJson/*.json` | 8 | Cross-promotion ad lists read by [HouseAds2](https://github.com/p32929/HouseAds2) and [MyHouseAdsAndroid](https://github.com/p32929/MyHouseAdsAndroid) |
| Other JSON | a few | Per-app data (BPL fixtures, Islamic content, plasma donors, etc.) |

Files are grouped into folders per app or per code-name (`Alpha/`, `Aizen/`, `DeSplash/`, `BuySellBD/`, …).

## How it's used

An app hardcodes a raw URL and fetches it, for example:

```
https://raw.githubusercontent.com/p32929/SomeHowTosAndTexts/master/HouseAdsJson/house_ads2.json
```

Editing a file here changes what every installed copy of that app sees, immediately — that's the whole point of keeping them out of the APK.

## Contributing

Contributions are warmly welcomed and greatly appreciated! Whether it's a bug fix, new feature, or improvement, your input helps make this project better for everyone.

Before submitting a pull request, please:

1. Create an issue describing the feature or bug fix you'd like to work on
2. Wait for discussion and approval to ensure alignment with project goals
3. Fork the repository and create your feature branch
4. Submit your pull request with a clear description of changes

This approach helps avoid duplicate efforts and ensures smooth collaboration. Thank you for considering contributing!

## Share

Sharing this repository with your friends is just one click away from here

[![facebook](https://user-images.githubusercontent.com/6418354/179013321-ac1d1452-0689-493f-9066-940cf2302b6e.png)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/p32929/SomeHowTosAndTexts/)
[![twitter](https://user-images.githubusercontent.com/6418354/179013351-7d8d6d1c-4ce2-46ab-bef8-4c4765a1b888.png)](https://twitter.com/intent/tweet?url=https://github.com/p32929/SomeHowTosAndTexts/)
[![tumblr](https://user-images.githubusercontent.com/6418354/179013343-3111f55a-3b90-40c7-8487-9777348672b0.png)](https://www.tumblr.com/share?v=3&u=https://github.com/p32929/SomeHowTosAndTexts/)
[![pocket](https://user-images.githubusercontent.com/6418354/179013334-b095c45f-becf-49f4-9ee1-5a731a9b1f85.png)](https://getpocket.com/save?url=https://github.com/p32929/SomeHowTosAndTexts/)
[![pinterest](https://user-images.githubusercontent.com/6418354/179013331-44cd9206-11b1-4b65-becb-5863b61c828f.png)](https://pinterest.com/pin/create/button/?url=https://github.com/p32929/SomeHowTosAndTexts/)
[![reddit](https://user-images.githubusercontent.com/6418354/179013338-7416ae3f-73ba-4522-86e1-1374d7082d22.png)](https://www.reddit.com/submit?url=https://github.com/p32929/SomeHowTosAndTexts/)
[![linkedin](https://user-images.githubusercontent.com/6418354/179013327-ca7b7102-1da8-4b1c-858f-1a6e5f21bd70.png)](https://www.linkedin.com/shareArticle?mini=true&url=https://github.com/p32929/SomeHowTosAndTexts/)
[![whatsapp](https://user-images.githubusercontent.com/6418354/179013353-f477fa0b-3e6f-4138-a357-c9991b23ff88.png)](https://api.whatsapp.com/send?text=https://github.com/p32929/SomeHowTosAndTexts/)

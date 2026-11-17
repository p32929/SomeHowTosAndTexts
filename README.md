# SomeHowTosAndTexts

The free file host behind my Android apps. It holds the JSON and HTML files that my apps download while they run, through `raw.githubusercontent.com`. Changing a file here changes what every installed copy of that app sees, straight away, with no app update and no server to pay for.

This is not a project you run. It is a place files are served from.

## What's in here

1. **Privacy policies and terms** (`privacy_policy.html`, `terms_and_conditions.html`, about 20 files): the pages each app links to, because Google Play needs a hosted link.
2. **Update checks** (`updater.json`, about 12 files): read by [AndroidAppUpdater](https://github.com/p32929/AndroidAppUpdater). Raise the version in one of these to ask that app's users to update.
3. **Cross-promotion lists** (`HouseAdsJson/*.json`, 8 files): the apps to advertise, read by [HouseAds2](https://github.com/p32929/HouseAds2) and [MyHouseAdsAndroid](https://github.com/p32929/MyHouseAdsAndroid).
4. **App data** (a few JSON files): content some apps load, like BPL 2019 fixtures, Islamic content and a plasma donor list.

Files are in one folder per app or per code name, for example `Alpha/`, `Aizen/`, `DeSplash/` and `BuySellBD/`.

## How an app uses it

The app has the raw link built in and downloads it, for example:

```
https://raw.githubusercontent.com/p32929/SomeHowTosAndTexts/master/HouseAdsJson/house_ads2.json
```

Edit the file here and push, and every copy of the app gets the new content the next time it loads the link.

## Contributing

Contributions are very welcome, thank you! Before you start on a pull request, please open an issue and tell me what you would like to add or change. That way we can agree on it first, and your time is not wasted on something that might not fit. Thanks for helping make SomeHowTosAndTexts better.

## You might also like

<a href="https://openstore.pfay.workers.dev/cards/p32929?n=4&amp;repo=SomeHowTosAndTexts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/cards/p32929.svg?n=4&amp;repo=SomeHowTosAndTexts&amp;theme=dark"><img src="https://openstore.pfay.workers.dev/cards/p32929.svg?n=4&amp;repo=SomeHowTosAndTexts&amp;theme=light" width="100%" alt="More apps by p32929 on OpenStore"></picture></a>

<p><a href="https://p32929.github.io/share/?repo=SomeHowTosAndTexts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-share-dark.svg"><img src="https://p32929.github.io/readme/footer-share-light.svg" width="50%" align="top" alt="Share this project with your friends in one click"></picture></a><a href="https://p32929.github.io/support/"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-support-dark.svg"><img src="https://p32929.github.io/readme/footer-support-light.svg" width="50%" align="top" alt="If you like my work and want to support me, feel free to support"></picture></a><br><a href="https://openstore.pfay.workers.dev/add"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-join-dark.svg"><img src="https://p32929.github.io/readme/footer-join-light.svg" width="100%" align="top" alt="Put your own apps on OpenStore: free, your listing lives in your own repo"></picture></a></p>

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

## Share

<a href="https://p32929.github.io/share/?repo=SomeHowTosAndTexts"><img src="https://p32929.github.io/readme/share.svg" alt="Share this with your friends in just a click" width="420"></a>

## Support

<a href="https://p32929.github.io/support/"><img src="https://p32929.github.io/readme/support.svg" alt="If you like my works and want to support me, feel free to support" width="420"></a>

#### Test Device
- [Set up a test device](https://support.google.com/admob/answer/9691433?hl=en#ID)
- How to find the advertising ID / IDFA of your device:

```
import AdSupport
print(ASIdentifierManager.shared().advertisingIdentifier)
// 76823A59-BF9D-46F7-840E-5A3EBB77882A
```

#### Authorize seller for app
- Helps protect your app ad inventory from ad fraud
- You create app-ads.txt files to identify who is authorized to sell your inventory
- Publish your app-ads.txt at the root of your developer website
- You can publish app-ads.txt with Firebase Hosting
- [Source](https://developers.google.com/admob/android/app-ads#firebase)

#### How to obtain EU consent
- You must have a **Funding Choices** account linked to your AdMob account.
- [Using UMP SDK](https://developers.google.com/admob/ump/ios/quick-start)
- [How IAB requirements affect EU consent messages](https://support.google.com/fundingchoices/answer/10207733)

#### Preparing for iOS 14+
- [Source](https://support.google.com/admob/answer/9997589?hl=en)

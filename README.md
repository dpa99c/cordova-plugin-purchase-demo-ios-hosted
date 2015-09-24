cordova-plugin-purchase-demo-ios-hosted
=======================================

Demo iOS in-app purchase XCode project for the [demo app](https://github.com/dpa99c/cordova-plugin-purchase-demo) of the [Cordova Purchase Plugin](https://github.com/dpa99c/cordova-plugin-purchase)

See the [iOS-specific documentation](https://github.com/dpa99c/cordova-plugin-purchase/blob/master/doc/ios.md#hosted-content) for details on how to use this project with the demo app.

This IAP package contains the content payload files within the `nonconsumablehosted1` subdirectory (alongside the ContentInfo.plist), but note that it doesn't matter if the payload files are place within this folder or alongside the xcodeproj file in the folder above, **so long as they have references created in the XCode project** - [see here](https://developer.apple.com/library/ios/recipes/xcode_help-structure_navigator/articles/Adding_an_Existing_File_or_Folder.html) for details how to do this.

This IAP uses the `<Folder>` key in the plist to specify a target folder with the same name as the IAP: `nonconsumablehosted1`. This means the payload files will be deployed to `{app ID}/Documents/nonconsumablehosted1/`; for example, `payload.txt` will be deployed to `{app ID}/Documents/nonconsumablehosted1/payload.txt`.
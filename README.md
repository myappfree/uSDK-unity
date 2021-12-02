# uSDK Unity Plugin

## Integration Guide
1. Import the AppsFlyer plugin package (https://github.com/AppsFlyerSDK/appsflyer-unity-plugin)
2. Import the Google External Dependency Manager package (you can usually skip this step, since the AppsFlyer plugin should import it for you) (https://github.com/googlesamples/unity-jar-resolver)
3. Import the uSDK Unity package
4. Select the "Assets/Create/MyAppFree/uSDK Config" menu item to create a new config file
5. Fill in the info of the config file
6. In a scene in your project, ideally the very first one to be loaded, create an empty Game Object, add the USDKController script to it, then set the USDKConfig property to the config file you created in step 4
7. Build your Unity project as usual

## Known Issues
- On iOS, the "Render Extra Frame on Pause" flag in the Player Settings might cause the uSDK plugin to fail to show the offer wall. There is currently no workaround to this, except disabling this behaviour.
- On iOS, AppsFlyer overrides the default Unity app controller. This might cause conflicts with other plugins that also override it. Should you encounter issues, enable the "iOS Swizzling" flag in the uSDK config file.
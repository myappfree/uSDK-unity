# uSDK Unity Plugin

## Integration Guide
1. Import the Google External Dependency Manager package (https://github.com/googlesamples/unity-jar-resolver)
2. Import the uSDK Unity package
3. Select the "Assets/Create/MyAppFree/uSDK Config" menu item to create a new config file
4. Fill in the info of the config file
5. In a scene in your project, ideally the very first one to be loaded, create an empty Game Object, add the USDKController script to it, then set the USDKConfig property to the config file you created in step 3
6. Build your Unity project as usual

## Known Issues
- On iOS, the "Render Extra Frame on Pause" flag in the Player Settings might cause the uSDK plugin to fail to show the offer wall. There is currently no workaround to this, except disabling this behaviour.

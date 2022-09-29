# React Native Navigation explained

notes are abridged from this link: https://reactnative.dev/docs/navigation

```
npm install @react-navigation/native @react-navigation/native-stack
npm install react-native-screens react-native-safe-area-context
```

For IOS

```
cd ios
pod install
```

## Trouble shooting

If there is an issue with the render such as "requireNativeComponent: "RNSScreenStackHeaderConfig" was not found in the UIManager when running android app"

```
https://stackoverflow.com/questions/69043806/requirenativecomponent-rnsscreenstackheaderconfig-was-not-found-in-the-uimana

I encountered this problem after setting up navigation for ios. Here is the solution I found:

In the terminal, run npx pod-install ios because as explained in the docs, "If you're on a Mac and developing for iOS, you need to install the pods (via Cocoapods) to complete the linking."
Quit my simulator
Terminated and re-ran npx react-native start
Terminated and re-ran npx react-native run-ios
After completing these steps the app ran successfully again.

```

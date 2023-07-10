This is a new [**React Native**](https://reactnative.dev) project, bootstrapped using [`@react-native-community/cli`](https://github.com/react-native-community/cli).

# Getting Started

>**Note**: Make sure you have completed the [React Native - Environment Setup](https://reactnative.dev/docs/environment-setup) instructions till "Creating a new application" step, before proceeding.

## Step 1: Start the Metro Server

First, you will need to start **Metro**, the JavaScript _bundler_ that ships _with_ React Native.

To start Metro, run the following command from the _root_ of your React Native project:

```bash
# using npm
npm start

# OR using Yarn
yarn start
```

## Step 2: Start your Application

Let Metro Bundler run in its _own_ terminal. Open a _new_ terminal from the _root_ of your React Native project. Run the following command to start your _Android_ or _iOS_ app:

### For Android

```bash
# using npm
npm run android

# OR using Yarn
yarn android
```

### For iOS

```bash
# using npm
npm run ios

# OR using Yarn
yarn ios
```

If everything is set up _correctly_, you should see your new app running in your _Android Emulator_ or _iOS Simulator_ shortly provided you have set up your emulator/simulator correctly.

This is one way to run your app — you can also run it directly from within Android Studio and Xcode respectively.

## Step 3: Modifying your ADs

1. run `npm install react-native-fbads --save
2. run `react-native link react-native-fbads` if you are using react-native version < 0.60
3. run `cd ios && pod install && cd ..` if you are using react-native version >= 0.60
4. if you're using android studio Add the following to your `android/app/build.gradle` file:
   ```
   dependencies {
      implementation project(':react-native-fbads')
   }
   ```
5. open `APP.js` on line 66 and 86 replace the `YOUR_PLACEMENT_ID` with your placement id specific to your Interstitial ADs placement id
6. Test your app on your device or emulator

<p align="center">
  <img width="480" src=".github/assets/logo-light.png#gh-light-mode-only" />
  <img width="480" src=".github/assets/logo-dark.png#gh-dark-mode-only" />
</p>

# Braze React SDK

Effective marketing automation is an essential part of successfully scaling and managing your business. Braze empowers you to build better customer relationships through a seamless, multi-channel approach that addresses all aspects of the user life cycle Braze helps you engage your users on an ongoing basis.

- [Braze User Guide](https://www.braze.com/docs/user_guide/introduction)
- [Initial React Native SDK Setup](https://www.braze.com/docs/developer_guide/platform_integration_guides/react_native/react_sdk_setup/)

## Braze Expo Plugin

If you're using Expo, you can install our plugin to integrate the React Native SDK without any native code. See the [Braze Expo Plugin Github](https://github.com/braze-inc/braze-expo-plugin) for more details.

## Running the Sample App

- `AppboyProject` - Contains the AppboyProject sample app with integration examples for the React Native bridge. This sample app integrates the iOS bridge via manual linking, and the iOS SDK via Cocoapods. It can
also optionally integrate the iOS bridge using Cocoapods via a local Podspec.

The following commands apply to both sample projects and use the `AppboyProject` directory as an example.

```zsh
cd AppboyProject/
yarn install

# In a separate tab:
cd AppboyProject/
npx react-native start
```

### iOS
Our sample app integrates the native Braze iOS SDK through [Cocoapods](https://guides.cocoapods.org/using/getting-started.html).

From the `AppboyProject` directory:
```zsh
sudo gem install cocoapods
cd ios/
pod install
cd ../
npx react-native run-ios
```

### Android
From the `AppboyProject` directory:
```zsh
npx react-native run-android
```

## Style
- Generally we try to mimic the Braze Web SDK's Javascript interface where appropriate.
- We use [eslint](http://eslint.org/) as our linter. From the root directory, run `npm run lint` to list errors or `npm run lint-fix` to automatically fix errors. To override the rules in the [`standard-react`](https://github.com/feross/eslint-config-standard-react) config, add `"rules"` in `.eslintrc.json`.

## Testing
- We use [jest](https://facebook.github.io/jest/) for testing the React SDK.
- Run the tests and code coverage report using `npm test`

# @hzblj/react-native-materials

[![npm](https://img.shields.io/npm/v/@hzblj/react-native-materials.svg)](https://www.npmjs.com/package/@hzblj/react-native-materials)
[![license](https://img.shields.io/npm/l/@hzblj/react-native-materials.svg)](./LICENSE)

React Native component for native Material effects — using SwiftUI `Material` on iOS and `RenderEffect` on Android for consistent blur and translucency.

## Features

- ✨ Native SwiftUI `Material` on iOS
- 🌀 Android `RenderEffect` support (API 31+)
- 📱 Consistent blur and translucency across platforms
- ⚡️ High-performance, platform-optimized rendering


## Screenshots

| iOS Light                                    | iOS Dark                           | Android Light                                        | Android Dark |
|----------------------------------------------|------------------------------------|------------------------------------------------------|--------------|
| ![iOS Light](./example/assets/ios-light.png) | ![iOS Dark](./example/assets/ios-dark.png) | ![Android Light](./example/assets/android-light.png) | ![Android Dark](./example/assets/android-dark.png) |

> _Screenshots above to show the effect on each platform and theme._

## Installation

```sh
yarn add @hzblj/react-native-materials
```

> **Note:** After installing, you need to prebuild your app to generate the native code. Run:
>
> ```sh
> npx expo prebuild
> ```
>
> This step is required for the native modules to be linked in your project.


## Usage

```tsx
import { MaterialView } from '@hzblj/react-native-materials'

<VStack>
    <MaterialView material="thin" style={StyleSheet.absoluteFill} />
    <Text>Material</Text>
</VStack>
```



## Props

| **Prop**   | **Type**                                                    | **Default** | **Required** | **Description**                                                                 |
|:-----------|:------------------------------------------------------------|:-----------:|:------------:|:-------------------------------------------------------------------------------|
| `material` | `'ultra-thin'` \| `'thin'` \| `'regular'` \| `'thick'` \| `'ultra-thick'` | `'regular'`  |   No        | Material                                       |
| `variant`  | `'light'` \| `'dark'`                                       |  auto       |    No        | Forces light/dark appearance. If not set, uses system color scheme.            |
| ViewProps  | [ViewProps](https://reactnative.dev/docs/view#props)        |    —        |    No        | All standard React Native View props.                                           |




## Native Implementations
- [iOS SwiftUI MaterialView.swift](./ios/MaterialView.swift)
- [Android MaterialView.kt](./android/src/main/java/com/janblazej/materials/MaterialView.kt)


## License
MIT

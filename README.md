FlatList, VirtualizedList, SectionList for React-Native < 0.43
--

This repository mimics the latest changes in React Native 0.43.

## Motivation
Currently, React-Native@0.43 depends on React@16.0.0-alpha6 which isn't yet supported by many libraries like Enzyme etc. Although, this version of RN brings us amazing list views: FlatList, VirtualizedList & SectionList. So there is a choice either to use 0.43 with its awesome lists or use 0.42 and being able to test your applications with Enzyme. Well, I choose both ;)

This package contains copied and adapted implementation of 0.43 list features to < 0.43 realms.

## Installation

- Install package using your favorite manager:

  ```sh
  yarn add react-native-list
  ```
  or
  ```sh
  npm add react-native --save
  ```

- Add `react-native-list` to your `providesModuleNodeModules`:

  - If you don't have `rn-cli.config.js`, create `rn-cli.config.js` in the root directory of your project:

  ```js
  module.exports = {
    getProvidesModuleNodeModules() {
      return [
        'react-native',
        'react-native-windows',
        'react-native-list',
      ];
    },
  };
  ```

  - If you already have `rn-cli.config.js`, add `react-native-list` to your `getProvidesModuleNodeModules` function or copy it from the snippet above.
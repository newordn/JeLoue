# JeLoue mobile app

# Table of content

- Tech stack and tools
- How to run the app on your machine
- Libraries and usage
- Conventions and code hygene
- Some userful links

---

# Teck stack and tools

**Development tools**

- Javascript ecosystem [Node](https://nodejs.org/) v14.5+
- Dependency management [Yarn](https://classic.yarnpkg.com/)
- Preferred IDE [Visual Studio Code](https://reactjs.org/), make sure you download the latest versions with the following extensions installed
  - prettier - code formatter
  - tslint
  - jshint
  - color highlight

**Frameworks and main dependencies**

- [react](https://reactjs.org/)
- [react-native](https://facebook.github.io/react-native/)
- [react-navigation](https://reactnavigation.org/)
- [mobx](https://mobx.js.org)
- [formik](https://github.com/jaredpalmer/formik)

**Other tools**

- [CompressJpeg](https://compressjpeg.com/) you can use this tool to compress jpeg img.
- [CompressPng](https://compresspng.com/) you can use this tool to compress png img.
- [Figma](https://www.figma.com/) all designs are made using Figma. Refer to this for styles. No screens and components should be developped without a preliminaty design uploaded to Figma
- [Android Studio](https://developer.android.com/studio/) used to run and test the app source code on Android devices.

**Serverless**
This app does not depend on any service. We use Firebase as backend

**Other dev dependencies**

- [typescript](https://www.typescriptlang.org) We do not use plain Javascript. Typescripts allows us to catch errors and provide fixes before we run the code.
- [tslint](https://palantir.github.io/tslint/) nice linter to enforce our code hygene rules
- babel
- yarn

# How to run the app on your machine

- Make sure you install all the tools specified in the previous section.
- clone the repository in your machine
- Make sure you save in a safe folder. **DO NOT GIVE ACCESS TO ANYONE NOT INVOLVED IN THIS PROJECT**
- open your terminal or command line pointing to the project root folder (where `package.json` is located)
- run `yarn` to install all dependencies

**Run on android**

- Open an android simulator device or connect an android device
- `yarn android` - run in Android emulator (note: required to open Android simulator up first)

When running the app, react native created a bundler on another terminal. This terminal shows the status of the js bundle server. This is basically how the JS code is sent to native thread on the device. You can start the bundler by running

`yarn start`

If the app does not behave properly i.e not loading and reporting errors, it might be due to an unstable bundler. You can clean the cache and reinstall all dependencies by running

`yarn clean`

# Libraries and usage

Here we will list all the libraries used in the app. To be updated.

# Conventions and code hygene

As we work we find ourselve agreeing on some conventions. They should all go here.

1 - We will use appText instead of react native's default text component
2 - The name of the branch should be in snake case, first word should be the issue type and the others the feature's name(ex: screen_sign_in).
3 - For every issues you will create a new branch
4 - The name of a screen should be the same name inside the issue description follow by .screen.tsx
5 - The convention 4 is applied to components, styles ...
6 - The name of an interface should be in camelCase but started with I
7 - Folder name should be in plural (ex : components)
8 - You should always try to reuse components instead of styles
9 - The name of a pull request should be the type of thhe issues:follow by the same name inside the issue description

# Some userful links

Documentation and other usefull links should go here

- [api](https://hold-management.herokuapp.com/) you can play with it right now because we're not in production mode
- [apollo client for integration](https://www.apollographql.com/docs/react/get-started/) to get started with react native + apollo client

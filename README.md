# MVMKR

### Movie maker and manager
this program respects and based on [electron-react-boilerplate](https://github.com/chentsulin/electron-react-boilerplate).
thanks for people creating and maintaining it.

<br/>

## Install

* **Note: requires a node version >= 7 and an npm version >= 4.**

First, clone the repo via git:

```bash
git clone https://github.com/kkiyama117/MVMKR.git
```

And then install dependencies with yarn.

```bash
$ cd MVMKR
$ yarn
```
**Note**: If you can't use [yarn](https://github.com/yarnpkg/yarn), run `npm install`.

## Run

Start the app in the `dev` environment. This starts the renderer process in [**hot-module-replacement**](https://webpack.js.org/guides/hmr-react/) mode and starts a webpack dev server that sends hot updates to the renderer process:

```bash
$ yarn dev
```

Alternatively, you can run the renderer and main processes separately. This way, you can restart one process without waiting for the other. Run these two commands **simultaneously** in different console tabs:

```bash
$ yarn run start-renderer-dev
$ yarn run start-main-dev
```

## Packaging

To package apps for the local platform:

```bash
$ yarn package
```

To package apps for all platforms:

First, refer to [Multi Platform Build](https://www.electron.build/multi-platform-build) for dependencies.

Then,
```bash
$ yarn package-all
```

To package apps with options:

```bash
$ yarn package -- --[option]
```

To run End-to-End Test

```bash
$ yarn build
$ yarn test-e2e
```

:bulb: You can debug your production build with devtools by simply setting the `DEBUG_PROD` env variable:
```bash
DEBUG_PROD=true npm run package
```

## How to keep your project updated with the boilerplate
```sh
git remote add upstream https://github.com/chentsulin/electron-react-boilerplate.git
```

Then, use git to merge some latest commits:

```sh
git pull upstream master
```

## Maintainers
[kkiyama117](https://hinatan.jp)

## License
MIT © [kkiyama117](https://hinatan.jp)

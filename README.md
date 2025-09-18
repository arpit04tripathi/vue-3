# vue-3

Learning Vue 3 with hands-on.
This template should help get you started developing with Vue 3 in Vite.

**table of contents**
- [vue-3](#vue-3)
- [Recommended IDE Setup](#recommended-ide-setup)
  - [Type Support for `.vue` Imports in TS](#type-support-for-vue-imports-in-ts)
  - [Customize configuration](#customize-configuration)
- [Project Setup](#project-setup)
- [Run localhost](#run-localhost)
    - [Sync checkout branch to latest chnages](#sync-checkout-branch-to-latest-chnages)
    - [Compile and Hot-Reload for Development](#compile-and-hot-reload-for-development)
    - [Lint with ESLint](#lint-with-eslint)
    - [Type-Check, Compile and Minify for Production](#type-check-compile-and-minify-for-production)
    - [Run Unit Tests with Vitest](#run-unit-tests-with-vitest)
    - [Run End-to-End Tests with Playwright](#run-end-to-end-tests-with-playwright)
- [Deploy to gh-pages](#deploy-to-gh-pages)
- [Additional Docs](#additional-docs)


# Recommended IDE Setup

- IDE - [VSCode](https://code.visualstudio.com/)
- Extensions
  - [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur)
  - Markdown

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

# Project Setup

- Clone the repo
- Install nvm [node version manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script)
- Install node with below commands

```sh
# install and uses node version from .nvmrc file
nvm use
# install packages from package.json
npm install
```

# Run localhost

### Sync checkout branch to latest chnages

```sh
scripts/localhost.sh;
git push;
```

```sh
git fetch --all -p; git pull; git status;
git merge origin/main;
git push;
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```

```sh
npm run format
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Playwright](https://playwright.dev)

```sh
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
npm run build

# Runs the end-to-end tests
npm run test:e2e
# Runs the tests only on Chromium
npm run test:e2e -- --project=chromium
# Runs the tests of a specific file
npm run test:e2e -- tests/example.spec.ts
# Runs the tests in debug mode
npm run test:e2e -- --debug
```

# Deploy to gh-pages

```sh
npm run deploy
```

# Additional Docs

- [Create New and Setup](./docs/README.md)

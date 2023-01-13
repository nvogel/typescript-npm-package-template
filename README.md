# typescript-npm-package-template

> A npm package template using TypeScript

## Features

- [Semantic Release](https://github.com/semantic-release/semantic-release)
- [TypeScript](https://www.typescriptlang.org/)
- [Jest](https://jestjs.io/)
- [ESLint](https://eslint.org/)
- [Prettier](https://prettier.io/)

## Getting started

### Set up your repository

**Click the "Use this template" button.**

Alternatively, create a new directory and then run:

```bash
curl -fsSL https://github.com/nvogel/typescript-npm-package-template/archive/main.tar.gz | tar -xz --strip-components=1
```

Replace `FULL_NAME`, `GITHUB_USER`, and `REPO_NAME` in the script below with your own details to personalize your new package:

```bash
FULL_NAME="John Smith"
GITHUB_USER="johnsmith"
REPO_NAME="my-cool-package"
sed -i.mybak "s/\([\/\"]\)(nvogel)/$GITHUB_USER/g; s/typescript-npm-package-template\|my-package-name/$REPO_NAME/g; s/Ryan Sonshine/$FULL_NAME/g" package.json package-lock.json README.md
rm *.mybak
```

### Add NPM Token

Add your npm token to your GitHub repository secrets as `NPM_TOKEN`.

**Remove everything from here and above**

---

# my-package-name

[![npm package][npm-img]][npm-url]
[![Build Status][build-img]][build-url]
[![Downloads][downloads-img]][downloads-url]
[![Issues][issues-img]][issues-url]
[![Semantic Release][semantic-release-img]][semantic-release-url]

> My awesome module

## Install

```bash
npm install my-package-name
```

## Usage

```ts
import { myPackage } from 'my-package-name'

myPackage('hello')
//=> 'hello from my package'
```

[build-img]: https://github.com/nvogel/typescript-npm-package-template/actions/workflows/release.yml/badge.svg
[build-url]: https://github.com/nvogel/typescript-npm-package-template/actions/workflows/release.yml
[downloads-img]: https://img.shields.io/npm/dt/typescript-npm-package-template
[downloads-url]: https://www.npmtrends.com/typescript-npm-package-template
[npm-img]: https://img.shields.io/npm/v/typescript-npm-package-template
[npm-url]: https://www.npmjs.com/package/typescript-npm-package-template
[issues-img]: https://img.shields.io/github/issues/nvogel/typescript-npm-package-template
[issues-url]: https://github.com/nvogel/typescript-npm-package-template/issues
[semantic-release-img]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-release-url]: https://github.com/semantic-release/semantic-release

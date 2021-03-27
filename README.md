# path-equal

![stability](https://img.shields.io/badge/stability-stable-brightgreen)
![version](https://img.shields.io/badge/version-1.0.1-blue)
![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)

> Core functionality forked from [unional/path-equal](https://github.com/unional/path-equal)

File paths in Unix and Windows are different.
During test, sometimes we want to compare if the file paths are the same.

Doing this comparison can get unwieldy.
But not doing it would means the project can only be develop in specific platform.

This library provides this comparison to check if the two paths are the same,
regardless of the running platform.

## Install

```text
npm install --save @moraj/path-equal
```

### Usage

```ts
import pathEqual from '@moraj/path-equal'

pathEqual('dir/sub-dir/file.txt', 'dir\\sub-dir\\file.txt') // true
```

This library will not access the file system,
so comparing absolute path with relative path will fail.

## Contribute

```sh
# after fork and clone
npm install

# begin making changes
git checkout -b <branch>
npm run watch

# after making change(s)
git commit -m "<commit message>"
git push

# create PR
```
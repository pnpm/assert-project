# @pnpm/assert-project

> Utils for testing projects that use pnpm

[![npm version](https://img.shields.io/npm/v/@pnpm/assert-project.svg)](https://www.npmjs.com/package/@pnpm/assert-project) [![Build Status](https://img.shields.io/travis/pnpm/assert-project/master.svg)](https://travis-ci.org/pnpm/assert-project)

## Install

pnpm install -D @pnpm/assert-project

## Usage

```ts
import test = require('tape')
import assertProject from '@pnpm/assert-project'

test('...', t => {
  // ...
  const project = assertProject(t, pathToProject)

  await project.has('foo')
  // Test fails if project has no foo in node_modules
})
```

## License

[MIT](./LICENSE) © [Zoltan Kochan](https://www.kochan.io/)

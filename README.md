[![Build Status](https://travis-ci.com/UnlyEd/utils-simple-logger.svg?branch=master)](https://travis-ci.com/UnlyEd/utils-simple-logger)
[![Maintainability](https://api.codeclimate.com/v1/badges/72c72fc8ca87933827a3/maintainability)](https://codeclimate.com/github/UnlyEd/utils-simple-logger/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/72c72fc8ca87933827a3/test_coverage)](https://codeclimate.com/github/UnlyEd/utils-simple-logger/test_coverage)

# Utils Simple Logger

Logger based on [Winston](https://github.com/winstonjs/winston) with sane default so that it only logs `error` in production and filter other logs, while keeping them all in non-production environments.

Basically avoids to increase cost by logging too much stuff in production.

<!-- toc -->

- [Getting started](#getting-started)
- [API](#api)
- [Contributing](#contributing)
  * [Getting started](#getting-started-1)
  * [Test](#test)
  * [Releasing and publishing](#releasing-and-publishing)
- [License](#license)

<!-- tocstop -->

## Getting started

npm or yarn

```
npm install @unly/utils-simple-logger
```

Use:

```
const logger = require('@unly/utils-simple-logger');
```

## API

[API](./API.md)

---

## Contributing

We gladly accept PRs, but please open an issue first so we can discuss it beforehand.

### Getting started

```
yarn start # Shortcut - Runs linter + build + tests in concurrent mode (watch mode)

OR run each process separately for finer control

yarn lint
yarn build
yarn test
```

### Test

```
yarn test # Run all tests, interactive and watch mode
yarn test:once
yarn test:coverage
```

### Releasing and publishing

```
yarn releaseAndPublish # Shortcut - Will prompt for bump version, commit, create git tag, push commit/tag and publish to NPM

yarn release # Will prompt for bump version, commit, create git tag, push commit/tag
npm publish # Will publish to NPM
```

## License

MIT

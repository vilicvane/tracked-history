[![NPM Package](https://badge.fury.io/js/tracked-history.svg)](https://www.npmjs.com/package/tracked-history)

# Tracked History

`BrowserHistory` tracks browser history so that we can restore history stack with snapshots.

> It was originally created for [Boring Router](https://github.com/makeflow/boring-router) to support complete lifecycle hooks while keeping browser navigation behavior right.

`MemoryHistory` and `ReadOnlyHistory` are also available for testing or server-side usages.

## Installation

```sh
npm install tracked-history
```

## Usage

```ts
import {BrowserHistory} from 'tracked-history';

const history = new BrowserHistory();

const snapshot = history.snapshot;

void history.push('/about');

void history.restore(snapshot);
```

## License

MIT License.

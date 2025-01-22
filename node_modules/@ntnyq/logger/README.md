# @ntnyq/logger

[![NPM VERSION](https://img.shields.io/npm/v/@ntnyq/logger.svg)](https://www.npmjs.com/package/@ntnyq/logger)

## Install

```bash
pnpm add @ntnyq/logger picocolors dayjs -D
```

## Usage

**default logger**:

```ts
import logger from '@ntnyq/logger'

logger.debug(`debug message`)
logger.info(`info message`)
logger.success(`success message`)
logger.warn(`warn message`)
logger.error(`error message`)
```

**custom logger**:

```ts
import { createLogger } from '@ntnyq/logger'

const logger = createLogger({ prefix: `[@ntnyq/logger]` })

logger.debug(`debug message`)
logger.info(`info message`)
logger.success(`success message`)
logger.warn(`warn message`)
logger.error(`error message`)
```

## Options

`createLogger` options:

### `prefix`

log prefix

**type**: `string`

**default**: ``

### `type`

show log type: `debug`, `info`, `success`, `warn`, `error`

**type**: `boolean`

**default**: `true`

### `mode`

if `prod`, `debug` message will not be shown

**type**: `dev | prod`

**default**: `dev`

### `enable`

set `false` to disable all log

**type**: `boolean`

**default**: `true`

### `time`

set `string` for time format.

set `false` to disable time.

set `true` to enable time with format `YYYY-MM-DD HH:mm:ss`.

**type**: `string | boolean`

**default**: `false`

## License

[MIT](./LICENSE) License © 2022-PRESENT [ntnyq](https://github.com/ntnyq)

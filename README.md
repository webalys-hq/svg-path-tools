<p align="center">
  <img alt="Path that SVG!" title="Path that SVG!" src="logo.svg" width="450">
</p>

<p align="center">
  Utilities to manipulate <code>path</code>, such as <code>parse</code> and <code>scale</code>.
  <br />
  [wip]
</p>

## Install

```zsh
yarn add path-utils
```

## Usage

```js
import { parse, scale, stringify } from 'path-utils'

const d = 'M15 10A5 5 0 0 1 10 15A5 5 0 0 1 5 10A5 5 0 0 1 15 10z'
const parsed = parse(d)
const scaled = scale(parsed, { scale: 0.5 })
const stringified = stringify(scaled)

// 'M7.5 5A2.5 2.5 0 0 1 5 7.5A2.5 2.5 0 0 1 2.5 5A2.5 2.5 0 0 1 7.5 5z'
```

## Related

[element-to-path](https://github.com/elrumordelaluz/element-to-path) Convert SVG element into `path`

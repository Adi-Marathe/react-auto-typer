# react-auto-typer

A lightweight auto-typer React component.

[![NPM](https://img.shields.io/npm/v/react-auto-typer.svg)](https://www.npmjs.com/package/react-auto-typer) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-auto-typer
```

## Usage

The package exports a named component `AutoTyper`.

```jsx
import React from 'react'
import { AutoTyper } from 'react-auto-typer'

function Example() {
  return (
    <AutoTyper
      text='Sample text here'
      delay={100} // optional, defaults to 100
      styleClass='autotyper' // optional CSS class applied to the <p>
      repeat={false} // optional, whether to restart typing after completion
      onlyOnce={false} // optional, if true, calls onComplete and stops
      onComplete={() => console.log('typing complete')} // optional callback
    />
  )
}
```

## Props

- `text` (string, required): Text to auto type.
- `delay` (number, optional): Delay between typing steps in milliseconds. Defaults to `100`.
- `styleClass` (string, optional): CSS class applied to the wrapping `<p>` element.
- `repeat` (boolean, optional): If `true`, typing restarts after reaching the end. Default `false`.
- `onlyOnce` (boolean, optional): If `true`, the component will call `onComplete` once and stop the interval.
- `onComplete` (function, optional): Callback invoked once when typing completes (used when `onlyOnce` is true).

## Example


## License

Apache-2.0 © [trishantpahwa](https://github.com/trishantpahwa)

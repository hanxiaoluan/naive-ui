<!--anchor:on-->

# Get Started

## Installation

First install it.

```bash
npm install --save-dev naive-ui
```

## Usage

Add the following lines in you entry point js file.

```js
import { createApp } from 'vue'
import naive from 'naive-ui'

// naive ui works with `vfonts` https://github.com/07akioni/vfonts
// you can use font from `vfonts` easily, for example:
// Generic Font
import 'vfonts/Lato.css'
// Monospace Fonts
import 'vfonts/FiraCode.css'
// then it works

const app = createApp()
app.use(naive)
```

## Import on Demand

Here is a minimal example.

```js
import { createApp } from 'vue'
import {
  // create naive ui
  create,
  // component
  NButton,
  // component style
  buttonLight,
  // locale
  zhCN
} from 'naive-ui'

const naive = create({
  locales: [zhCN],
  styles: [buttonLight],
  components: [NButton]
})

const app = createApp()

app.use(naive)
```
<p align="center">
  <a href="https://google.com/">
    <img src="./docs/stamp_logo.png" alt="Stamp logo" width="auto" height="135">
  </a>
</p>

<h1 align="center">@stamp/react <code style="font-size: 15px;">v1.0</code></h1>

<p align="center">
  Generic React components to use as building blocks for your PostNL UI
  <br>
    <br>
  <a href="Link naar zeroheight?"><img src="./docs/explore_react_docs.svg" alt="Stamp logo" width="auto" height="38"></a>
  <a href="Link naar zeroheight?" class="stamp-button stamp-button--variant-primary">Click dgbrnrtnrtnrtnrtnrt</a>
  <br>
  <br>
  <a href="link naar Slack?">Report bug (GitHub)</a>
  ·
  <a href="link naar Slack?">Request feature (GitHub)</a>
</p>

## Table of contents

- [Installation](#installation)
- [Getting Started](#getting-started)
- [Examples](#examples)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [Versioning](#versioning)
- [Copyright and license](#copyright-and-license)


## Installation

Stamp/react is available as an NPM package.

**Install with NPM:**

```bash
npm install @stamp/react
```

**Install with Yarn:**

```bash
yarn add @stamp/react
```

## Getting started
### Components

Here is an example of a basic app using Stamp/react `Button` component:

```jsx

import { Button, ThemeProvider } from '@stamp/react';

function App() {
  return (
  	<ThemeProvider>
  		<Button variant="secondary">Hello World</Button>;
  	</ThemeProvider>
  )
}
```

For more options and other components, read the React documentation.

[![Edit Button](./docs/read_documentation.svg)](link zero height)


### CSS

CSS is provided through a global stylesheet. An example of it's usage could be to import it in your JS application so styles are applied to the used components:

```js
import '@stamp/react/style.css';
```

To apply global styling, wrap your application in the `ThemeProvider` component:

```js
import { ThemeProvider } from '@stamp/react';
```

### Fonts

The `ThemeProvider` applies the `PostNL` font family to it's wrapping element. That font family needs to be made available to make those styles work. These fonts are located in the package at `dist/fonts`, and in the situation where you can link to assets from npm packages (e.g. webpack), it can be set up like this:

```css
@font-face {
    font-family: PostNL;
    src: url(@stamp/react/fonts/PostNL-Bold-Italic.woff2) format('woff2');
    font-weight: 700;
    font-style: italic;
}

@font-face {
    font-family: PostNL;
    src: url(@stamp/react/fonts/PostNL-Bold.woff2) format('woff2');
    font-weight: 700;
    font-style: normal;
}

@font-face {
    font-family: PostNL;
    src: url(@stamp/react/fonts/PostNL-Medium-Italic.woff2) format('woff2');
    font-weight: 400;
    font-style: italic;
}

@font-face {
    font-family: PostNL;
    src: url(@stamp/react/fonts/PostNL-Medium.woff2) format('woff2');
    font-weight: 400;
    font-style: normal;
}

@font-face {
    font-family: PostNL;
    src: url(@stamp/react/fonts/PostNL-Light-Italic.woff2) format('woff2');
    font-weight: 300;
    font-style: italic;
}

@font-face {
    font-family: PostNL;
    src: url(@stamp/react/fonts/PostNL-Light.woff2) format('woff2');
    font-weight: 300;
    font-style: normal;
}
```

## Examples
Naar zero height verwijzen waar per component voorbeeld staat?

[![Examples Button](./docs/show_examples.svg)](link zero height)

## Documentation
Naar zero height verwijzen ?

[![Docs Button](./docs/read_documentation.svg)](link zero height)

## Tools

### Vite

To distribute this component library, it needs to be bundled properly. [Vite](https://vitejs.dev/) bundles the library into the desired formats: esm & umd. This serves both modern and legacy usages.

To bundle the application using [Vite](https://vitejs.dev/), run the following command:

```bash
npm run build
```

### Storybook

[Storybook](https://storybook.js.org/) is used to preview isolated components

To run it using a development server, run the following command:

```bash
npm run storybook:start
```

To build a static version of it, run the following command:

```bash
npm run storybook:build
```

### Plop

Creating and adjusting files for new components can be painful. We've made this easier for you by using [Plop](https://plopjs.com/). To generate files for a new component, run the following command:

```bash
npm run generate
```

This prompts you to enter the name of the component and goes through the following steps:

-   Scaffolds a component directory containing the following files:
    -   Component file
    -   Barrel file where everything can be exported
    -   Style declarations
    -   Storybook story
-   Updates all barrel files in the package so the component is exported correctly

### Jest

For unit testing [Jest](https://jestjs.io) is used. To execute the tests, run the following command:

```bash
npm run test
```

## Contributing
### Help improve Stamp!
**Bug** <br>
If you find a bug, please let us know via the [... GitHub]()

**Feature request** <br>
If want to request a new feature, please let us know via the [... GitHub]()

## Versioning
?

<style>
	.stamp-button, .stamp-button {
	    display: inline-flex;
	    gap: 8px;
	    align-items: center;
	    justify-content: center;
	    max-inline-size: 100%;
	    inline-size: auto;
	    cursor: pointer;
	    padding-block: 8px;
	    padding-inline: 24px;
	    border-style: solid;
	    border-width: 1px;
	    font-family: PostNL;
	    font-weight: 500;
	    line-height: 1.5;
	    font-size: 16px;
	    -webkit-text-decoration: none;
	    text-decoration: none;
	}
	
	.stamp-button:hover {
	    -webkit-text-decoration: underline;
	    text-decoration: underline;
	}
	
	.stamp-button--variant-primary, a.stamp-button--variant-primary {
	    background-color: #3440b6;
	    border-color: #ffffff00;
	    border-radius: 24px;
	    color: #ffffff
	}
	
	.stamp-icon--size-s {
	    inline-size: 16px;
	    block-size: 16px;
	}
	
	.stamp-icon {
	    display: flex;
	}
</style>

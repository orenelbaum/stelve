# Stelve

Stelve is a cybernatically enhanced compiler for SloidJS. Sloid is great when you want to build large scale apps, but sometimes you just want something more concise that makes creating websites more enjoyable and more cybernetical.

Stelve is essentially a language that compiles to SloidJS. It's a language that is designed to be concise and easy to use. It's also designed to be cybernatically enhanced, meaning that it can be used to create cybernatically enhanced websites.


## Installation

Stelve is available on npm. You can install it with the following command:

```bash
npm install -g stelve
```


## Usage

Stelve is a command line tool. You can use it to compile your Stelve files to SloidJS files. You can also use it to compile SloidJS files to Stelve files.

### Compiling Stelve to SloidJS

To compile a Stelve file to a SloidJS file, you can use the following command:

```bash
stelve compile <input> <output>
```

### Compiling SloidJS to Stelve

To compile a SloidJS file to a Stelve file, you can use the following command:

```bash
stelve decompile <input> <output>
```


## Syntax

Stelve is the most concise language in the world, and as such, it has a very simple syntax. Here is a quick overview of the syntax:

### Variables

In Stelve you don't need to declare variables. You can just use them. Here is an example:

```stelve
a=1
```

Notice how there is no space between the variable name and the equals sign. This is because Stelve is designed to be concise, and as such, it doesn't allow any unnecessary whitespace.

This will compile to the following SloidJS:

```js
// index.js
import appRenderer from "./renderer.js";

appRenderer.renderApp();

```

```jsx
// renderer.jsx
import { useHook, useRender } from "sloid";
import Root from "./root.jsx";

function renderApp() {
	useHook([useRender], ([useRender]) => {
		useRender([Root], () => {
			return <Root />;
		});
	});
}

const appRenderer = {
	renderApp,
};

export default renderApp;

```

```jsx
// Root.jsx
import { useHook, useComponent, useRoot } from "sloid";
import App from "./App.jsx";

const Root = useHook([useComponent], ([useComponent]) => {
	useComponent([useRoot], () => {
		useRoot([App], () =>{
			return <App />;
		});
	});
});

export default Root;

```

```jsx
// App.jsx
import { useHook, useComponent, useSnigal } from "sloid";

const Root = useHook([useComponent], ([useComponent]) => {
	useComponent([useSnigal], () => {
		const [a, setA] = useSnigal(1);
		return <>{null}</>;
	});
});

```

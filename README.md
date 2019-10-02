# Create React App Minimal setup

`cra-minimal` runs `create-react-app` and then replaces the contents of the `src/`
folder with my preferred minimal boilerplate. Read more in the About this program section below.

## Usage

Install `create-react-app`:

```bash
npm install -g create-react-app
```

Install `cra-minimal`:

```bash
npm install -g https://github.com/arthurbernierjr/create-react-app-minimal
```

Use `cra-minimal` as you would use `create-react-app` to create a project:

```bash
cra-minimal my-new-react-project
```

Uninstall if you don't like it:

```bash
npm uninstall -g cra-minimal
```

## About this program

I 💚 create-react-app, but I don't always want the boilerplate files that it comes with:

```
src/
├── App.css
├── App.js
├── App.test.js
├── index.css
├── index.js
├── logo.svg
└── registerServiceWorker.js
```

This program runs `create-react-app` and replaces the contents of the `src`
folder with [my preferred boilerplate](./minimalSrcContent):

```
src/
├── App.css
├── App.js
└── index.js
```

### `App.css` (empty file)

```css
```

### `App.js`

```js
import React, { Component } from "react";
import "./App.css";

class App extends Component {
    render() {
        return <div className="App">Hello World</div>;
    }
}

export default App;
```

### `index.js`

```js
import React from "react";
import ReactDOM from "react-dom";
import App from "./App";

ReactDOM.render(<App />, document.getElementById("root"));
```

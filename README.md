# A boilerplate to start create a Typescript SDK 

## HTML

```html
<script src="./index.js">
    ExampleSDK.foo()
</script>
```

## React

```js

// 1. Download React
yarn getReact

// 2. Build the SDK for both client/node, and publish locally using yalc
yarn build

// 3. Go to the React app and link the local published sdk (change the name of the package name `sdk-ts-starter` to something you desired)
yarn linkReact

// 4. In the App.js
import * as ExampleSDK from 'sdk-ts-starter';
ExampleSDK.hello();

```

# Yarn commands

> `devHtml`: Listens to Typescript file changes from `src`, and output to `src_build_from_ts`, which is also being listend and built to `./build/web/index.js`. Finally, run a live server on `localhost:3000` 

> `devReact`: Listens to Typescript file changes from `src`, and output to `src_build_from_ts`, which is also being listend and built to `./build/node/index.js`. Finally, run React app on `localhost:3000` 
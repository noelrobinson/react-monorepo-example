# Monorepo Structure

```
| packages/
| -- apps/
| ---- app-1/
| ------ index.js
| ------ package.json
| ---- app-2/
| ------ index.js
| ------ package.json
| -- components/
| ---- comp-1/
| ------ index.js
| ------ package.json
| ---- comp-2/
| ------ index.js
| ------ package.json
| ---- comp-3/
| ------ index.js
| ------ package.json
| package.json
| lerna.json
```

The monorepo is using [lerna](https://lerna.js.org/) and [yarn workspaces](https://classic.yarnpkg.com/en/docs/workspaces/) together

# Running Storybook

From the project root

```
npm run storybook
```

This will pick up the stories configured in .storybook/main.js


example used with some modifications as i couldnt get `babel-loader-lerna-cra` to work with create react app 2

https://itnext.io/guide-react-app-monorepo-with-lerna-d932afb2e875

# Hot Reloading

So changes to the components will hot reload when runnning as a dependancy within the react app. 
Hot reloading will also work with Storybook


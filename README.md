# ESLint config

## Whats included?

- Standard config base;
- React plugin;
- React Hooks plugin;
- JSX a11y plugin;
- Prettier;

## Setup

### React (with Next.js)

Install dependencies:
```sh
npm i -D eslint fredmarques/eslint-config
```
Inside `.eslintrc.json`
```json
{
  "extends": [
    "fredmarques/eslint-config/next", 
    "next/core-web-vitals"
  ]
}
```

### React (without Next.js)

Install dependencies:
```
npm i -D eslint fredmarques/eslint-config
```
Inside `.eslintrc.json`
```json
{
  "extends": "fredmarques/eslint-config/react"
}
```

### Node.js

Install dependencies:
```sh
npm i -D eslint fredmarques/eslint-config
```
Inside `.eslintrc.json`
```json
{
  "extends": "fredmarques/eslint-config/node"
}
```

## Editor setup

### vscode
Be sure you have the [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) extension installed. Uninstall prettier extension if you have it installed.

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.formatOnSave": false
}
```

### Credits
This settings were inspired on [@RocketSeat's repo](https://github.com/Rocketseat/eslint-config-rocketseat)
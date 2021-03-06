# eslint-config-hermez

This repo contains a shareable ESLint config to share across all the frontend projects in the Hermez
organization. It has been designed to work with TypeScript and React.

This config will ignore common directories in a React project created with `create-react-app`:

- `node-modules`
- `build`
- `public`

# Setup

First of all, you will need to install the `peerDependencies`:

```sh
npm i react typescript eslint
```

After that, you'll be able to install the package without warnings:

```sh
npm i @hermeznetwork/eslint-config-hermez
```

Then, create an `.eslintrc.json` file in your frontend project with this content:

```json
{
  "extends": "@hermeznetwork/eslint-config-hermez"
}
```

Check that everything works fine:

```sh
eslint --ext .ts,.tsx .
```

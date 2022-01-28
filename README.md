<div align="center">
  <h1><code>brightsign-webpack</code></h1>
  <p><strong>Webpack + React + Typescript + Tailwind</strong></p>
</div>

## Install

Run `yarn` in the repository root.

## Development

See [`package.json`](./package.json) scripts. TypeScript's `tsc` can be run with
`yarn tsc`.

### Webpack

- Both JavaScript and Typescript modules will work and are interoperable.
- [`swc`](https://swc.rs/docs/configuration/compilation) is used to transpile
  JS/TS, see `ecmaVersion` in the webpack config.
- BrightSign modules (`@brightsign/...` imports) are automatically included in
  webpack externals. If more externals are needed, see
  [combining syntaxes](https://webpack.js.org/configuration/externals/#combining-syntaxes).

### TypeScript

- Add a `@ts-expect-error` comment above BrightSign module imports (see
[`node/api.ts`](./node/api.ts)).

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

Before creating a production version of your app, install an [adapter](https://kit.svelte.dev/docs#adapters) for your target environment. Then:

```bash
npm run build
```

> You can preview the built app with `npm run preview`, regardless of whether you installed an adapter. This should _not_ be used to serve your app in production.

## Troubleshooting
> Cannot read properties of undefined (reading 'rimraf')

edit `node_modules\@sveltejs\adapter-static\index.js`

change to `async adapt( utils )`

https://giters.com/sveltejs/kit/issues/1602

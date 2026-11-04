# seha-sa

React and Vite application restored from the source archive.

## Development

Install dependencies with `npm ci`, then run `npm run dev`.
Run `npm run lint` to check TypeScript.

## Netlify deployment

`netlify.toml` configures the production command and publishes `dist`.
The SPA rewrite serves `index.html` for client-side routes, including direct visits and page refreshes.
Static images and other assets are served from `public`.

## Existing application limitations

The archived application uses browser local storage for its records and accounts.
Its Vite development-only API was not a production backend and was not restored.
This deployment repair does not add server-side persistence or authentication.
Embedded default login credentials were omitted from the restored source.

# Template from Netlify + Solid

![Netlify + Solid](https://user-images.githubusercontent.com/43764894/223558736-6cf48156-2316-419d-8be9-e318ecf0e4be.png)

## Project Structure

```
/
├── public/
│   └── favicon.ico
├── src/
│   ├── components/
│   │   └── Counter.css
│   │   └── Counter.tsx
│   └── routes/
│       └── [...404].tsx
│       └── index.tsx
├── entry-client.tsx
├── entry-server.tsx
├── root.css
├── root.tsx
├── package.json
└── vite.config.json
```

## Getting Started

If you want to get started locally, you can clone the project, install the dependencies and run the dev command!

```
git clone https://github.com/netlify-templates/solid-quickstart.git
cd solid-quickstart
npm install
npm run dev
# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

Solid apps are built with _adapters_, which optimise your project for deployment to different environments.

By default, `npm run build` will generate a Node app that you can run with `npm start`. To use a different adapter, add it to the `devDependencies` in `package.json` and specify in your `vite.config.js`.

## Deploying using the Netlify CLI
- Install the Netlify CLI globally `npm install netlify-cli -g`
    
- Run `npm run build`

- Then use the `netlify deploy` for a deploy preview link or `netlify deploy --prod` to deploy to production

Here are a few other ways you can deploy this template:
    
- Use the Netlify CLI's create from template command `netlify sites:create-template solid-quickstart` which will create a repo, Netlify project, and deploy it
    
- If you want to utilize continuous deployment through GitHub webhooks, run the Netlify command `netlify init` to create a new project based on your repo or `netlify link` to connect your repo to an existing project

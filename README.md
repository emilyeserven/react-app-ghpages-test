I just wanted a template for some React and Tailwind that's deployable to GitHub pages.

## Important Commands
- `npm run dev` - Runs locally
- `npm run deploy` - Deploys to GitHub pages

## Initial Setup

- To change the URL the repo can be accessed from, change `base` value in `vite.config.ts`.
- Make sure to visit the repo's GitHub Pages settings and set it to deploy from the `gh-pages` branch (which may only be visible after an initial deploy).
- In the index file, or something like `main.tsx`, make sure URLs are relative. ([See example here](https://github.com/emilyeserven/parse-n-plot/commit/3f2d773d89b74f2290385553c3526d13112caa2c))

## Created using...

- https://tailwindcss.com/docs/guides/vite
- https://dev.to/rashidshamloo/deploying-vite-react-app-to-github-pages-35hf

---

_Following is the default README_

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:
- 
- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list

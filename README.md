# vite-react-tailwind-template
Use Vite + React + Tailwindcss like flash.

# once upon a time i tiped in the terminal when i created this template
## First, i installed vite with react  as a template

```bash
yarn create vite my-app --template react
```

## .then, taiwindcss with his friends

```bash
yarn tailwindcss@latest postcss@latest autoprefixer@latest -D
```
## .then make config: 
### mkdir a postcss.config.js file at the root of your project
    // postcss.config.js
    module.exports = {
      plugins: {
        tailwindcss: {},
        autoprefixer: {},
      }
    }

### Create your configuration file

```bash
npx tailwindcss init
```
### .then make config for tailwindcss

      // tailwind.config.js
      module.exports = {
        mode: "jit",
        purge: ['./src/**/*.{js,jsx,ts,tsx}', './public/index.html'],
        darkMode: false, // or 'media' or 'class'
        theme: {
          extend: {},
        },
        variants: {},
        plugins: [],
      }

### .then i included Tailwind in my CSS in ./src/index.css file

    /* ./src/index.css */
    @tailwind base;
    @tailwind components;
    @tailwind utilities;


## and then ...
All this has already happened 🏆, I'm just telling the story. The thing that remains to be done is to

```bash
cd vite-react-tailwind-template && yarn dev
```

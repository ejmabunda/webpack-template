# webpack-template

A modern, minimal, and reusable webpack template for quickly bootstrapping new JavaScript projects. This template provides a solid foundation with separate development and production configurations, automatic HTML generation, and a clean build process.

## Features

- 📦 Modular Webpack configuration (common, development, production)
- ⚡ Development server with live reload (via `webpack-dev-server`)
- 🧼 Clean output directory on each build
- 🏗️ Automatic HTML file generation (`HtmlWebpackPlugin`)
- 🔗 Source maps for easier debugging (inline in dev, external in prod)
- 🛠️ Easy to extend for styles, images, and more

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ejmabunda/webpack-template.git
cd webpack-template
```

### 2. Install dependencies

```bash
npm install
# or
yarn install
```

### 3. Project structure

```
webpack-template/
├── dist/                 # Bundled output (auto-generated)
├── src/
│   └── index.js          # Project entry point
├── package.json
├── webpack.common.js
├── webpack.dev.js
├── webpack.prod.js
└── README.md
```

### 4. Running the development server

```bash
npm start
# or
yarn start
```

Runs the app in development mode.
Open [http://localhost:8080](http://localhost:8080) to view it in the browser.

### 5. Building for production

```bash
npm run build
# or
yarn build
```

Creates a `dist` folder with your production build.

## Customization

- **Entry Point:** Change the `entry` property in `webpack.common.js`.
- **HTML Title:** Edit the `HtmlWebpackPlugin` config in `webpack.common.js`.
- **Add CSS, images, or Babel:** Extend `webpack.common.js` with additional loaders and plugins as needed.

## Extending this Template

- Add CSS/SASS support with `style-loader`, `css-loader`, and `sass-loader`.
- Add Babel for ES6+ or React support.
- Add asset/resource handling for images and fonts.
- Integrate ESLint, Prettier, or Jest as needed.

## License

[MIT](LICENSE)

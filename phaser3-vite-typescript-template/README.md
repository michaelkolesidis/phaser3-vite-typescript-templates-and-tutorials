# Phaser 3 + Vite + TypeScript Template

Make Phaser 3 games modern frontend tooling.

## Prerequisites

You'll need [Node.js](https://nodejs.org/en/), [npm](https://www.npmjs.com/) and [Yarn](https://classic.yarnpkg.com/lang/en/) installed.

It is highly recommended to use [Node Version Manager](https://github.com/nvm-sh/nvm) (nvm) to install Node.js and npm.

If Yarn is not installed, you can install it globally with:

```
npm install -g yarn
```

## Getting Started

Install dependencies:

```
yarn
```

Start development server:

```
yarn dev
```

To create a production build:

```
yarn build
```

Production files will be placed in the `dist` folder. Then upload those files to a web server. 🎉

## Project Structure

```
    .
    ├── dist
    ├── node_modules
    ├── public
    ├── src
    │   ├── HelloWorldScene.ts
    │   ├── main.ts
	├── index.html
    ├── package.json
    ├── tsconfig.json
    ├── vite.config.ts
```

TypeScript files are intended for the `src` folder. `main.ts` is the entry point referenced by `index.html`.

Other than that there is no opinion on how you should structure your project.

There is an example `HelloWorldScene.ts` file that can be placed inside a `scenes` folder to organize by type or elsewhere to organize by function. For example, you can keep all files specific to the HelloWorld scene in a `hello-world` folder.

It is all up to you!

## Static Assets

Any static assets like images or audio files should be placed in the `public` folder. It'll then be served from the root. For example: http://localhost:8000/images/my-image.png

Example `public` structure:

```
    public
    ├── images
    │   ├── my-image.png
    ├── music
    │   ├── ...
    ├── sfx
    │   ├── ...
```

They can then be loaded by Phaser with `this.image.load('my-image', 'images/my-image.png')`.

## Acknowledgments

Based on the template provided by [Tommy Leung (supertommy)](https://github.com/supertommy).

## License

Copyright (c) 2023 Michael Kolesidis

[MIT License](https://github.com/ourcade/phaser3-vite-template/blob/master/LICENSE)

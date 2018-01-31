# Wijmo JavaScript UI Controls by GrapeCity

- [Official Wijmo website](https://www.grapecity.com/en/wijmo)
- [Free Wijmo trial download](https://www.grapecity.com/en/download/wijmo-enterprise)

Build lightweight, high-performing HTML5/JavaScript apps with zero dependencies, fast. Deliver next-generation HTML5 applications with this award-winning collection of true JavaScript controls written in TypeScript and built for speed.

## Getting Started

    npm install "git+https://github.com/cgatno/wijmo-eval.git"

If you're building a React app, for example:

    import { FlexGrid } from 'wijmo/wijmo.react.grid';
    
    ...

    render() {
      return (
        <div>
          <FlexGrid />
        </div>
      );
    }

## Why is this on GitHub?

This repository hosts the latest evaluation version of Wijmo's minified, obfuscated CommonJS modules. For almost all use cases, you should [download the trial version of Wijmo from the official website](https://www.grapecity.com/en/download/wijmo-enterprise).

This repo exists, however, to make it easy to install the Wijmo trial using [npm](https://npmjs.org) and incorporate it into projects with [Node.js](https://nodejs.org/en/)-powered tooling. For example, you can use this to easily try out Wijmo controls in a React app bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

You can also use this setup to create apps using Wijmo on sites like [Glitch](https://glitch.com).

## Licensing

Note that the usage of this repository and the Wijmo code contained within is governed by the [GrapeCity EULA](https://www.grapecity.com/en/legal/eula). Especially, you may not obscure or remove the Wijmo watermark that displays when the controls are loaded. View the [LICENSE](LICENSE) file for comprehensive licensing rules.

If you want to use Wijmo in a production environment, purchase a license on the [GrapeCity website](https://www.grapecity.com/en/pricing#wijmo).

## Wijmo README Content

```
Npm image for Wijmo CommonJS modules (minified)
===============================================

This folder represents an npm image containing Wijmo core and Angular 2 interop 
modules in CommonJS module format, and corresponding TypeScript definition (.d.ts) files.
The folder also includes metadata files for Angular 2 AoT compiler (.metadata.json).

<b>NOTE:</b> despite the ".min" suffix is not present in .js file names, these files are MINIFIED. 
The ".min" suffix is omitted in order to simplify modules usage in conjunction with 
various application bundlers and loaders, where mapping of ambient module names used in 
applications (like "wijmo/wijmo.grid") to minified file names having ".min.js" extension 
requires either an additional setup or even not possible in some tools.

Because the folder content is formed as an npm image, you can easily install it in your 
application using "npm install <path_to_folder>" command in NodeJS command prompt, like this:
npm install ../wijmo_download/NpmImages/wijmo-commonjs-min
This command will add the folder content to the node_modules/wijmo folder of your application.

Alternatively, you can add the following record to the package.json file of your application:
"dependencies": {
   "wijmo": "../wijmo_download/NpmImages/wijmo-commonjs-min",
   � other libraries
}
After that, each time you execute "npm install" command in your application root folder, 
Wijmo modules will be installed under the "node_modules" folder along with other libraries 
enumerated in package.json.
```

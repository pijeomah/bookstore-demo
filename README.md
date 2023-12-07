# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

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


To start the project type npm create vite
 Then npm install to install dependenecies 
 then type npm run dev to run the program 

 Then sanitize the project by deleting unnecessary files


 All CSS files and App.TS

 
//import Bootstrap
// implement folder structure
//create components folder
//create pages folder
//create utilities folder
//create hooks folder
//Create data folder
//create context folder
//All folders should be in src folder


First thing to do 
Wrap entire app with browser router tag from react-router-dom in main.tsx
import routes and route from rect router dom in the App.tsx file

import container comp from react-bootstrap in same App file

Wrap text with the container comp

The next step would be to create our routes in the App.tsx 

Inside the routes comp we need to crate a rout for each page each with an element and path prop

The path prop would hold the path for the file and the element prop would hold the file for that path
The next step would be to create all those files in the Pages folder
In each file create a simple function for each page that holds the text that holds the title of the page

In App.tsx import the files from the pages folder into the file

Using bootstrap styling set margin(mb-4) to the container

The next step is to build a navbar comp using bootstrap
In the components folder we create navbar.tsx
in App comp we import the navbar comp into the file


Add a fragment into the App function
 Above the Container add the self closing Navbar comp


 In the NAvbar comp export a simple Navbar function

 import bootstrap custom navbar but give it an alias 

 Inside the navbar function we input a navbar comp and inside an navbar comp input the container comp
 
 Apply appropriate Bootstrap styling here 
 refer to video
 
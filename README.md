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
 

 Next we create navbar links, inorder to do that  we connect the links to the router that is already set up foreach link using page Nav and Nav.Link comp
 Next we add a shopping cart button

 Inside the the Nav Container add a class name that pushes nav item to end of page
(refer to video)

Copy shopping cart button from github
Clear all unmade EH from the Button 

Now we create the data for our store in the Data folder with a json file called items copied from Github

The next thing to do is to import the json file into the Store file 

Next in the store function
we need to loop through the store items in the Json file the first step would be to wrap everything in a fragment, next would be to Wrap the mapped contents in a row and then loop through them using a map method then in the col comp in the map we stringify the store items
After this we apply some grid styling refer to 2h32m 

Next step would be to get rid of the stringified file in the Col comp and replace with a StoreItem file that has not yet been created 

In the components folder we create StoreItem withe props for name,id,price,imgUrl

we then create types for each of these props and then apply the type to the function


Next we use the custom bootstrap card comp to wrap all the info we are going to display for each store item

Then using the Card.img comp we apply the img to the store page
There is some styling here refer to the video at 
2h53m - 2h56m

Next we use the Card.Body for the part of the card that would hold the item name and price inside the body we use the card.Title to hold the actual string which would be in a span element there is styling here too
Next we format the prices 

To format the prices we create a new file in the utils folder and then we create the formatCurrency function 
After creating the function we wrap the function around the price all inside the curly brackets

The next step would be to hard code a quantity to test the functionality of adding items to the cart
Below the Card.Title comp create a div that holds the conditional that determines the visual state of the button
Apply styling referred from 3h25m -3h30m

Then we wrpa the tow seperate conditionals in aprentheses and in the second parentheses we create two divs one for adding and removing items and one for  
Next we test whether the codition works by manually testing the quantity

After testing we create two Buttons that would hold +/- signs with text between then a span should hold the text with a div wrapping it 
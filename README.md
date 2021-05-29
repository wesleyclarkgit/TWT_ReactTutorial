### Notes
5/29 Video #2
## Public Folder
Manifest gives a description of the application.  
We don't really need to mess with the public folder much
You can replace the logos and flavicon, but do change the places where logo is referenced if so.
Also, the icon must be renamed flavicon.ico for it to work



## SRC Folder
This is where the source code goes
Anything bundled up by webpack goes here
You could add another folder, like Components for organization purposes when project gets larger
Index.js
importing several libraries, style sheets and application
The lines



ReadtDom.render(
        <React.StrictMode>
        </React.StrictMode>
            <App />
        </React.StrictMode>,
        document.getElementById('root')
);

Render the main react component, App.  App is an example of a component
We are rendering app inside of document.getElementByID('root')
This means we are finding the root div inside the index.html file
and then injecting App inside of that div

In this tutorial we deleted reportWebVitals.js.  I don't know what that file is or what it does.  Follow up here!

# Index.js can be thought of as the entry point for the React application.  It takes our main component and renders it inside the html document



# App.js
This is the main component, and first thing that is rendered inside of the div.  It will render
other components.  It can be thought of as the main react app.

App.js returns HTML... not quite.  It's actually JSX that's going to be rendered inside that div.
Notice that in the div we are using className instead of class, that's JSX syntax.
JSX enables you to write native JavaScript into the HTML



App.css
CSS to be applied to app



Index.css
Currently set up as global css



App.test.js
Allows you to run automated tests for the application
This will let you know if the test ran successfully



setuptest.js
This sets up the testing environment by importing a library



package.json
Defines dependencies for application
If you install a dependency it's automatically installed here
Contains build, test and eject scripts.  You could create your own script if you wanted and add it here



Readme gives info about default app



gitignore
This will automatically initialize an empty git repository.  
Gitignore will stop a ton of files from being transferred



Nodemodules
This is where all the dependencies are located.  Hundreds of megabytes
If you were to delete this file, you could recreate all the dependencies by 'npm i'.  
This will automatically read package.json and reinstall them for us



webpack
Webpack is an open-source JavaScript module bundler.  It is made primarily for JavaScript, 
but it can transform front-end assets such as HTML, CSS, and images if the corresponding loaders
are included
It will take source code and bundle all of it into one large JavaScript file.  This makes it more efficient
to serve and run.  This happens on the backend, more info is beyond scope


Babel
Babel is a free and open-source JavaScript transcompiler that is mainly used to convert ECMAScript 2015+ code into
a backwards compatible version of JavaScript that can be run by older JavaScript engines.
Babel essentially enables your JavaScript to be compatible with any browser that is being used


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

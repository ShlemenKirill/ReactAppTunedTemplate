# React App Tuned Template
![CI/CD](https://github.com/ShlemenKirill/ReactAppTunedTemplate/workflows/CI/CD/badge.svg)
[![Codecov](https://img.shields.io/codecov/c/github/ShlemenKirill/ReactAppTunedTemplate)](https://app.codecov.io/gh/ShlemenKirill/ReactAppTunedTemplate)
[![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT)
[![CodeQL](https://github.com/ShlemenKirill/ReactAppTunedTemplate/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ShlemenKirill/ReactAppTunedTemplate/actions/workflows/codeql-analysis.yml)

This is a solution template for creating a React App with tuned ES lint and Prettier. Create a new project based on this template by clicking the above **Use this template** button.

## Project structure

```
├── README.md
├── node_modules
├── .eslintrc
├── package.json
├── .gitignore
├── .prettierrc
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
    └── components
    │   ├── actions 
    │   ├── constants
    │   └── reducers
    └── constants
    └── pages
    └── store
    └── translations
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js
    └── setupTests.js
```

### ES lint configuration

``` javascript
{
	"env": {
		"browser": true,
		"jest/globals": true
	},
	"extends": ["airbnb", "prettier"],
	"plugins": ["prettier", "jest", "react-hooks"],
	"parser": "babel-eslint",
	"rules": {
		"prettier/prettier": "error",
		"import/no-extraneous-dependencies": [
			"error",
			{
				"devDependencies": true
			}
		],
		"import/no-named-as-default": 0,
		"react-hooks/rules-of-hooks": "error",
		"react-hooks/exhaustive-deps": "warn",
		"react/jsx-indent": "off",
		"react/jsx-indent-props": "off",
		"react/jsx-one-expression-per-line": "off",
		"react/jsx-wrap-multilines": "off",
		"capitalized-comments": [
			"error",
			"always",
			{
				"ignoreConsecutiveComments": true
			}
		],
		"react/jsx-props-no-spreading": "off",
		"react/jsx-curly-newline": "off",
		"jsx-a11y/control-has-associated-label": "off",
		"react/prop-types": 0,
		"react/forbid-prop-types": 0
	},
	"settings": {
		"import/resolver": {
			"node": {
				"moduleDirectory": ["node_modules", "src"]
			}
		},
		"import/ignore": [".css$"]
	}
}

```
### Prettier config
``` javascript
{
  "trailingComma": "es5",
  "tabWidth": 4,
  "useTabs": true,
  "semi": true,
  "singleQuote": true,
  "overrides": [
    {
      "files": "*.css",
      "options": {
        "tabWidth": 2,
        "useTabs": false
      }
    }
  ]
}

```

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

Create React App template and practice with eslint & prettier setup

download these under dev dependencies: 

touch .prettierrc; touch .eslintrc; yarn add -D eslint-config-airbnb eslint-config-prettier eslint-plugin-jsx-a11y eslint-plugin-prettier prettier; cd src; touch index.js; mkdir components; cd components; touch App.js; cd ../..

add .eslintrc

{
  "extends": [
    "react-app",
    "airbnb",
    "plugin:jsx-a11y/recommended",
    "prettier",
    "prettier/react"
  ],
  "plugins": ["jsx-a11y", "prettier"],
  "rules": {
    "semi": 1,
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],
    "prettier/prettier": ["error"]
  }
}

add .prettierrc

{
  "tabWidth": 2,
  "singleQuote": true,
  "semi": true,
  "trailingComma": "es5",
  "printWidth": 85,
  "arrowParens": "always"
}


shift command p 
  developer:reload window

check App.js page for prettier check mark and eslint connection on bottom dashboard

doc: 
  https://medium.com/@pppped/extend-create-react-app-with-airbnbs-eslint-config-prettier-flow-and-react-testing-library-96627e9a9672

prettier options/rules: 
  https://prettier.io/docs/en/options.html

eslint rules: 
  https://eslint.org/docs/rules/

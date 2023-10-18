# eslint_prettier_config

1.npm install eslint --save-dev

2.npm init @eslint/config
? How would you like to use ESLint? ... => To check syntax, find problems, and enforce code style
? What type of modules does your project use? => JavaScript modules (import/export)
? Which framework does your project use? => React
? Does your project use TypeScript? => No
? Where does your code run? => Browser
? How would you like to define a style for your project? => Use a popular style guide
? Which style guide do you want to follow? => Airbnb: https://github.com/airbnb/JavaScript
? What format do you want your config file to be in? => JSON
? Would you like to install them now with npm? => Yes

3.npm install --save-dev --save-exact prettier

4.npm install --save-dev eslint-config-prettier

5.npm install --save-dev eslint-plugin-prettier

6.  Create ".eslintignore" and ".prettierrc" files

7.  In file ".eslintignore" add names of folders that must be ignored:
    node_modules
    build
    public

8.  In file ".prettierrc" add object:
    {
    "trailingComma": "es5",
    "tabWidth": 3,
    "semi": false,
    "singleQuote": true,
    "endOfLine": "auto"
    }

9.  In file ".eslintrc.json" to key "rules" add object:
    {
    "react/jsx-filename-extension": [
    1,
    {
    "extensions": [".js", ".jsx"]
    }
    ],
    "react/jsx-props-no-spreading": "off",
    "react/react-in-jsx-scope": "off",
    "import/prefer-default-export": "off",
    "no-use-before-define": "off",
    "no-shadow": "off",
    "react-hooks/exhaustive-deps": "off",
    "react/function-component-definition": "off",

         "max-len": [
            "error",
            {
               "code": 100,
               "ignoreStrings": true,
               "ignoreTemplateLiterals": true,
               "ignoreRegExpLiterals": true
            }
         ],
         "no-console": ["warn", { "allow": ["warn", "error"] }],

         "react-hooks/rules-of-hooks": "error",

         "jsx-a11y/label-has-associated-control": [
            "error",
            {
               "required": {
                  "some": ["nesting", "id"]
               }
            }
         ],
         "no-param-reassign": [
            "error",
            { "props": true, "ignorePropertyModificationsFor": ["state"] }
         ],
         "prettier/prettier": ["error", { "singleQuote": true, "parser": "flow" }],
         "react/destructuring-assignment": ["off"],
         "react/prop-types": ["off"],
         "jsx-a11y/no-noninteractive-element-interactions": ["off"],
         "jsx-a11y/click-events-have-key-events": ["off"],
         "react/button-has-type": ["off"],
         "consistent-return": ["error"],
         "jsx-a11y/media-has-caption": ["off"],
         "no-constant-condition": "off"
         }

10. In file ".eslintrc.json" to key "plugins" replace object: ["react", "react-hooks"],

1.10. In file ".eslintrc.json" to key "extends" replace object:
[
"plugin:react/recommended",
"airbnb",
"plugin:prettier/recommended"
],

12.If you don't have installed Eslint and Prettier extensions - YOU NEED TO INSTALL THEM!
And after you need reload your VSCode and enjoy to coding!

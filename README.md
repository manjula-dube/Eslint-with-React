

# ESLint Rules for React

Code style is an important topic for developers. When you code for yourself, it might be alright to violate best practices. However, in a team of developers you have to have a common code style. You should follow the same rules to make your code look alike. It helps others developers to read your code. It helps people to navigate in a new code base. ESLint in JavaScript helps you to set up rules and to enforce code style.

Let’s add some code style checking for React. Therefore you need to add the eslint-plugin-react.

From root folder:

* ` npm --save-dev install eslint-plugin-react `

Now you can use the react plugin and specify your first React rule, which says that you have to specify PropTypes for your React components.

In you .eslintrc file do the following

```
{
  parser: "babel-eslint",
  "plugins": [
    "react"
  ],
  "rules": {
    "max-len": [1, 120, 2, {ignoreComments: true}],
    "prop-types": [2],
    'no-console': 0, // we are enabling this in the scripts
		'no-debugger': 0, // we are enabling this in the scripts
  }
}
```

When you start your app, you might see: Definition for rule 'prop-types' was not found. You might want to fix them by defining PropTypes for your React components. It will also error saying that "Unexpected console statement" & "Unexpected debugger statement"

These were your first custom JavaScript and React rules. But you can use common recommendations from the community. Such presets, like they exist for React, give you a set of rules that everyone uses.

```
{
  parser: "babel-eslint",
  "plugins": [
    "react"
  ],
  "rules": {
    "max-len": [1, 120, 2, {ignoreComments: true}],
    "prop-types": [2]
  },
  "extends": ["eslint:recommended", "plugin:react/recommended"]
}
```


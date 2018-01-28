

# ESLint Rules for React

Code style is an important topic for developers. When you code for yourself, it might be alright to violate best practices. However, in a team of developers you have to have a common code style. You should follow the same rules to make your code look alike. It helps others developers to read your code. It helps people to navigate in a new code base. ESLint in JavaScript helps you to set up rules and to enforce code style.

Let’s add some code style checking for React. Therefore you need to add the eslint-plugin-react.

From root folder:

* ` npm --save-dev install eslint-plugin-react `

Now you can use the react plugin and specify your first React rule, which says that you have to specify PropTypes for your React components.

In you .eslintrc file do the following





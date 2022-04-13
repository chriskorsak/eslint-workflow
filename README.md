# ESLint WORKFLOW

## Background

ESLint is a tool for identifying and reporting on patterns found in JavaScript code, with the goal of making code more consistent and avoiding bugs.

ESLint can enforce a consistent style across a team of developers if a project has this installed as a dependency. This makes collaboration easier and it makes the code more readable for everyone.

You can 'lint' manually by running a script in the terminal, and you can also have linting run before the build process. In the latter case, if there is a linting error, it won't complete the build until the error is fixed.

## Add ESLint as a dev dependency

- Initialize npm in project directory: `npm init -y` in terminal
- Install dependency in project directory: `npm i eslint --save-dev`
- Create an eslint config file (go through prompt questions about project). Either command works:
  - `npm init @eslint/config`
  - `npx eslint --init`
- Create a script in package.json: `"lint": "eslint src"` src is where you want to run the linting. It can be whatever you want for the path of project.
- To lint your files, you can now run `npm run lint` in the terminal
- You can go through the eslint config step again if you want to change things, like adding a popular style guide to a project. This might be a better idea rather than manually adjusting the .eslintrc.js file.

## Using ESLint in real time in a text editor

- If you have the ESLint plugin installed in VS Code (or other text editor), and you have gone through the above steps to add ESLint as a dependency, the plugin will then lint your JS files in real time in VS Code.
- However, it's also possible to globally install ESLint, rather than as a dependency in a project, but this is not recommended. In other words, you would have a global .eslintrc.js configuration, rather than a project-specific one.

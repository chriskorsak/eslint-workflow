# ESLint WORKFLOW

## Add ESLint as a dev dependency

- Initialize npm in project directory: `npm init -y` in terminal
- Install dependency in project directory: `npm i eslint --save-dev`
- Create an eslint config file: `npm init @eslint/config` (go through prompt questions)
- Create a script in package.json: `"lint": "eslint src"` src is where you want to run the linting. It can be whatever you want for the path of project.
- To lint your files, you can now run `npm run lint` in the terminal
- You can go through the eslint config step again if you want to change things, like adding a popular style guide to a project. This might be a better idea rather than manually adjusting the .eslintrc.js file.

## Using ESLint in real time in a text editor

- If you have the ESLint plugin installed in VS Code, and you have gone through the above steps to add as a dependency, the plugin will then lint your JS files in real time as you code.
- However, it's also possible to globally install ESLint, rather than as a dependency in a project, but this is not recommended.

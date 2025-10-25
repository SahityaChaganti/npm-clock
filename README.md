# 🕒 Digital Clock using Moment.js

A simple digital clock application built using **JavaScript**, **Moment.js**, and **npm**.  
It displays the current time dynamically and updates every second.

## 🚀 Features

- Displays real-time clock with hours, minutes, and seconds
- Uses Moment.js for time formatting
- Lightweight and responsive
- Demonstrates npm package usage in a small project

## 🛠️ Tech Stack

- JavaScript
- HTML / CSS
- Moment.js (via npm)

- What is npm ?

npm (Node Package Manager) is a tool which manages packages for Javascript projects
it helps us to install, update, and share reusable code
comes automatically with nodejs

- Some common command:

npm init -- Initializes the a project and creates packagge.json
npm install -- Installs all dependencies listed in package.json
npm install <package> -- Install specific package locally
npm install -g <package> -- Install specific package globally
npm run <script> -- Runs the custom script inside package.json
npm list -- lists all installed packages

- Undestanding package.json

It tells the npm which projects are needed
project name, version
commands to run the script.
For example:
{
"name": "weather-app",
"version": "1.0.0",
"scripts": {
"start": "react-scripts start",
"build": "react-scripts build"
},
"dependencies": {
"react": "^18.0.0",
"axios": "^1.4.0"
},
"devDependencies": {
"jest": "^29.0.0"
}
}

- Dependencies vs DevDependencies

Dependencies. -- needed for app to run -- example react,axios

DevDependencies. -- used only during development -- example jest,eslint,webpack
example:
npm install package-name # → dependency
npm install package-name --save-dev # → devDependency

- Package-lock.json
  locks exact version of installed packages.
  recreated automatically when run npm install.

💬 Common npm Questions (with answers)
🏷️ 1. What is npm, and why is it used?

npm stands for Node Package Manager. It’s used to manage JavaScript packages — installing, updating, and managing dependencies.

⚙️ 2. What is the difference between dependencies and devDependencies?

dependencies are required to run the app, while devDependencies are only needed for development (testing, linting, etc.).

📘 3. What is the purpose of package.json?

It contains metadata about the project and defines dependencies, scripts, and versions for consistent builds.

🔒 4. What is package-lock.json and why is it important?

It ensures deterministic builds by locking specific dependency versions, preventing version mismatches across environments.

🧑‍💻 5. What’s the difference between global and local packages?

Local: Installed in your project (node_modules folder).

Global: Installed system-wide and available everywhere.

Example:

npm install -g typescript

🚀 6. How do you create a new React app using npm?

Run:

npx create-react-app my-app

(npx comes with npm; it runs packages without installing them globally.)

🧹 7. What is npx?

npx executes packages directly from npm without permanently installing them. Useful for one-time commands like create-react-app.

🧪 8. What happens when you run npm install?

npm checks package.json and installs all dependencies into the node_modules folder.

⚠️ 9. What is semantic versioning in npm (^ and ~)?

^1.2.3 → allows minor and patch updates (1.x.x)

~1.2.3 → allows patch updates only (1.2.x)

1.2.3 → fixed version

🧰 10. How can you update all npm packages at once?
npm update

or check outdated ones:

npm outdated

# IZSoftware/ Web FrontEnd Onboarding Project
The purpose of this project is to provide new hire with a place to learn and familiarize themselves
with project structure of web front-end apps within the organization.
## Technologies used and prerequisites
You should have good understanding of git from the [IZ training course](https://izsoftwares.atlassian.net/wiki/spaces/~712020639e69eca7b4437c994612b8ff80e0a0/pages/16252953/IZ+Training+Course) as well as the following web front-end specific techologies:
- [React](https://react.dev/learn)
- [Typescript](https://www.typescriptlang.org/docs/)
- [Tailwind](https://tailwindcss.com/docs/installation)

Optionally you can learn a little about:
- [Prettier](https://prettier.io/) (for code formatting)
- [Eslint](https://eslint.org/) (to ensure consistent code style)


## Development Environment Setup
1. Download and install [nodejs](https://nodejs.org/)
2. Install yarn by running `npm install -g yarn`
3. Download and install [git](https://git-scm.com/downloads)
4. You have created a [git account](https://github.com/signup) and been invited to the team organization.
5. Download and install [vscode](https://code.visualstudio.com/)
   - vscode is the only code editor being used across the web front-end team.
6. In vscode install the following extensions if you haven't alreay:
   - ESlint (by microsoft); This will allow you to format code properly with `Ctrl+F`
   - Tailwind CSS IntelliSence (by Tailwind labs); This will give you intellisence for tailwind css classes.
   -  Simple React Snippets (by Burke Holland); This is optional but is a good extension for react snippets.
## Starting a new project
To start any new project, you should clone the starter template and start any work from the template. To do so:
1. Clone the git project
```bash
git clone https://github.com/IZEPR/iz-website-starter-template.git
```
2. Cd into cloned directory and install packages
```bash
cd iz-website-starter-template
yarn install
```
1. Delete .git directory within iz-website-starter-template to start a new git project
## Onboarding project
Now that you are all setup let's get started on the actually meat of the onboarding project. For this project you are going to use the website-starter-template to create a front-end app. Please follow these [rules](#Considerations-when-working-in-a-project) when working on projects.


The app should use a REST API to send requests and show the data or do some computation and display a result. This project should take no more than a week please choose wisely. Here are some basic project ideas to consider:

1. A currency exhange rate app that implements certain 10 or more currencies
   - Possible API if you want to investigate thiss https://www.exchangerate-api.com/docs/free
  
2. Star wars search app; Can search by keyword and filter by type.
   -  Possible API if you want to investigate this https://swapi.dev/

3. A Joke telling app; Generate a Joke depending on some context
   - Possible API if you want to investigate this https://sv443.net/jokeapi/v2/#getting-started

4. Github profile searching app; search profile and list some user's projects
   - Possible API if you want to investigate this https://docs.github.com/en/rest/quickstart

After going through this exercise please create a new branch and create a pull request.

## Considerations when working in a project
### Style considerations
- Use camelCase not snake_case for variable, function, classes, etc...
- filenames in camelCase for components.
### Code organization
- File types in respective folders.
  - assets in `src/assets`
    - This means for example images are in src/assets/images
    - Font styles are in src/assets/fonts etc..
  - styles and CSS in `src/styles`
    - css relevant for a component should be in a file named after the component name. For instance styles for the Button component should be in src/styles/Button.css

- Organization of code depending on intent:
  - simple components in `src/components` folder
  - higher order components in `src/hoc` folder
  - custom hooks in `src/hooks` folder
  - routes components in `src/routes` or `src/pages` folder
  - library code in `src/lib` folder
  - common/utility code in `src/utils` 
- To check linting errors use `yarn lint` and to fix the errors `yarn lint:fix`

### ALWAYS tests
- Every component created should have a unit test named after itself in the `src/tests` folder. For example Button component should have a the file src/tests/Button.test.tsx for it's test.

---
Please *DONOT* hesitate to report and ask questions in case of doubt this is a learning project afer all. 

---
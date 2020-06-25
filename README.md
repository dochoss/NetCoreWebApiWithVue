# .Net Core 3.1 Web API with Vue JS (No TypeScript)

Template with .Net Core 3.1 Web Api with a VueJS client without TypeScript.

# To Get Started
- clone
- cd ClientApp
- npm install

# Installed Features
- Axios for Http
- Vue 
  - Vue Router
  - Vuex
- `package.json` added to root project folder for easy running of Vue's npm scripts with Task Runner Explorer in Visual Studio
  - These are just mirrors of the default Vue-CLI scripts (serve, build, lint) with `cd ClientApp && ` added in front of each command.


If you want to change your API routes, make sure to update `axios.defaults.baseURL` in ClientApp/src/main.js

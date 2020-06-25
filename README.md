# .Net Core 3.1 Web API with Vue JS (No TypeScript)

Template with .Net Core 3.1 Web Api with a VueJS client without TypeScript.

This template is based on [aspnetcore-vueclimiddleware](https://github.com/EEParker/aspnetcore-vueclimiddleware) by Github user EEParker.  It didn't get included in the default template selection for Visual Studio, which is a shame, but the code is still provided in the repo.

# Changes to Base
- Moved `WeatherForecase.cs` to the `Models` folder
- Added Axios NPM library to the Vue project
- Set baseURL for Axios in Vue `main.js` file to match default web API controller route (`/api`)
- Added required dotnet package for VueCliMiddleware

# To Get Started
- _clone_
- cd ClientApp
- npm install
- cd ..
- dotnet run -p NetCoreWebApiWithVue.csproj

# Installed Features
- Axios for Http
- Vue 
  - Vue Router
  - Vuex
- ES Lint (default Vue-CLI configuration)
- Node-Sass (default Vue-CLI configuration)

- `package.json` added to root project folder for easy running of Vue's npm scripts with Task Runner Explorer in Visual Studio
  - These are just mirrors of the default Vue-CLI scripts (serve, build, lint) with `cd ClientApp && ` added in front of each command.


If you want to change your API routes, make sure to update `axios.defaults.baseURL` in ClientApp/src/main.js.  Existing setup uses .Net Core default of `/api/<endpoint>`

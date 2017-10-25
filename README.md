# coosto-interview

[![Standard - JavaScript Style Guide](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

> My first Vue.js app, coded during a technical interview! 😎

## Assignment

Create a todo application in Vue. The API is available at http://weslezw230.230.axc.nl/notes. We would recommend you to use the `vue­-cli`, which can be retrieved from [here](https://github.com/vuejs/vue­cli).

This application is going to be deployed in a corporate environment. The interviewers are the
stakeholders/ product owners.

### API endpoints

CMD | Endpoint | Comments
--- | --- | ---
GET | http://weslezw230.230.axc.nl/notes
GET | http://weslezw230.230.axc.nl/notes/@id | (returns full post)
POST | http://weslezw230.230.axc.nl/notes | (only returns a message)
PUT | http://weslezw230.230.axc.nl/notes | (only returns a message)
DELETE | http://weslezw230.230.axc.nl/notes | (only returns a message)

We’re going to assess you on the reasoning behind the decisions. The goal is not to have a fully functional working application (but would be awesome), we’re much more interested in the way you set up the project and what your thoughts are when building an application from scratch.

If you think something is a good idea, but you don’t see any room to fit this in this timebox, please make a remark in your code that that still should be done.

## Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

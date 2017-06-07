# heroku

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test

# deploy to heroku
npm deploy
```

## Steps to deploy
1. npm install -g vue-cli
2. vue init webpack my-project
3. cd my-project
4. npm install
5. npm run build
6. Create package.json in /dist
7. Create server.js in /dist
8. Test by going to cd dist and npm start
9. git init
10. git add . & git commit -m 'first commit'
11. heroku git:remote -a vue-deploy-example
12. Remove /dist from .gitignore
13. git status --short
14. git add . & git commit -m 'adding dist files'
15. heroku buildpacks:set heroku/nodejs
16. git subtree push --prefix dist heroku master

## Sources
- [How to deploy Vue Webpack to Heroku](https://medium.com/@sagarjauhari/quick-n-clean-way-to-deploy-vue-webpack-apps-on-heroku-b522d3904bc8)
- [VueJs Webpack](http://vuejs-templates.github.io/webpack/)
- [Docs for vue-loader](http://vuejs.github.io/vue-loader)

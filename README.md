#Angular + Express + Heroku Starter app

## Project setup

This project is already configured for deploying on Heroku, following their instructions.
See it running at: https://angular-express-starter-2017.herokuapp.com/

You can get to https://angular-express-starter-2017.herokuapp.com/api/test to try the Express routing

Project is based on the tutorial at https://devcenter.heroku.com/articles/mean-apps-restful-api.
A few changes had to be made in order for it to successfully deploy to Heroku, that the tutorial misses to explain or maybe changed since then.
Some of them:

1. Added these instructions to Package.json (inside "scripts"):
"preinstall": "npm install -g @angular/cli",
"postinstall": "ng build --prod"

2. Had to move the Angular-Cli dependencies from devDependencies in order for Heroku to be able to run "ng" commands 
"@angular/cli": "^1.3.2",
"@angular/compiler-cli": "^4.4.3",

More instructions to come.

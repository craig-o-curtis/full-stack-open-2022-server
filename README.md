# Server-side code

Client-side code at [https://github.com/craig-o-curtis/full-stack-open-2022](https://github.com/craig-o-curtis/full-stack-open-2022)

Heroku:

- [https://uhel-demo-app.herokuapp.com](https://uhel-demo-app.herokuapp.com)
- [https://uhel-2022-server.herokuapp.com/api/contacts](https://uhel-2022-server.herokuapp.com/api/contacts)

## Scripts

```bash
npm start               // node index.js
npm run dev             // nodemon index.js
npm run heroku:local    // heroku local web
npm run build:ui        // rm -rf build && cd ../full-stack-open-2022-client/ && npm run build && cp -r build ../full-stack-open-2022-server
npm run deploy          // git push heroku main
npm run deploy:full     // npm run build:ui && git add . && git commit -m uibuild && npm run deploy
npm run logs:prod       // heroku logs --tail
```

## Backend Setup

### Heroku

Setup steps are at [https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up](https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up)

Sign up for a Heroku account [Heroku](https://devcenter.heroku.com/)

Install Heroku

```bash
brew install heroku/brew/heroku
```

Log in

```bash
heroku login
```

Start locally with

```bash
heroku local web
```

Create a Heroku app with

```bash
heroku create -a uhel-2022-server
```

// https://uhel-demo-app.herokuapp.com/ | https://git.heroku.com/uhel-demo-app.git

Push to Heroku

```bash
git push heroku main
```

Deployed to:
https://uhel-demo-app.herokuapp.com
https://uhel-demo-app.herokuapp.com/api/contacts

Check Heroku logs with:

```bash
heroku logs -t
```

// step 3.10 confirms works at https://uhel-2022-server.herokuapp.com
// step 3.11 confirms works on Heroku and locally

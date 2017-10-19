This repo is for the creator of react-twitter-auth to reproduce an issue I'm having.

The original example repo is [here](https://github.com/GenFirst/react-node-twitter-login)

To reproduce the error:
1. clone repo, build and run as per original instructions (below).
2. Click twitter auth button and twitter auth appears in popup window.
3. Press ctrl-shift-i to bring up dev tools console and you will see the warning
about semi-colon ';' is invalid separator.
4. Click authorise button.
5. Popup window stays open and displays app - whereas it should really hide itself I think.
6. Note the ```console.log( "@twitter response on success");``` in client app.js
onSuccess function doesn't appear in (either) console.


# react-node-twitter-login

Demo application that shows how implement Twitter login with React on frontend and Node.js/Express on backend that is implementing REST API.

# About

This application was created as material that is described in the [blog post](https://medium.com/@robince885/how-to-do-twitter-authentication-with-react-and-restful-api-e525f30c62bb).
For creating React app we have used [crate-react-app](https://github.com/facebookincubator/create-react-app).

# What you need to install

* [Node.js](https://nodejs.org/en/)
* [crate-react-app](https://github.com/facebookincubator/create-react-app)
* [Gulp](http://gulpjs.com/)
* [MongoDB](https://www.mongodb.com/)

# How To Start Application?

* Start MongoDB - our application expects that there is `twitter-demo` database in MongoDB
* Put Twitter secret and key in [passport.js](https://github.com/GenFirst/react-node-twitter-login/blob/master/backend/passport.js) and [server.js](https://github.com/GenFirst/react-node-twitter-login/blob/master/backend/server.js) files
* Go to [frontend](https://github.com/GenFirst/react-node-twitter-login/tree/master/frontend) folder
    * `npm install`
    * `npm start`
* Go to [backend](https://github.com/GenFirst/react-node-twitter-login/tree/master/backend) folder
    * `npm install`
    * `gulp develop`

# License

react-node-twitter-login is released under [MIT License](https://opensource.org/licenses/MIT).

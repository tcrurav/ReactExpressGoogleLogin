# React (frontend) and Express (backend) Example using OAuth2 with Login

This project is just a project example to learn how to use OAuth2 Login with Google using ReactJS (frontend) and Express (backend).

This example is just a copy from https://www.sitepoint.com/google-auth-react-express/

## OAuth2 explained with 2 Diagrams

This diagram has been taken from https://blog.prototypr.io/how-to-build-google-login-into-a-react-app-and-node-express-api-821d049ee670. Is a good way to understand the OAuth2 flow used in this project.

![screenshots](https://github.com/tcrurav/ReactExpressGoogleLogin/blob/master/screenshots/OAuth2Diagram-2.png)

This other flow diagram is taken from https://medium.com/javarevisited/jwt-and-social-authentication-using-spring-boot-90e4faaa9204. This project doesn't implement this diagrama. But I include it here because It's a good way to understand the following step you will have to do when you implement OAuth2 in a more complete way:

![screenshots](https://github.com/tcrurav/ReactExpressGoogleLogin/blob/master/screenshots/OAuth2Diagram.png)

## Getting Started

Download links:

You can start by the original version of this project: https://www.sitepoint.com/google-auth-react-express/

## Prerequisites

You need a working environment with:
* [Git](https://git-scm.com) - You can install it from https://git-scm.com/downloads.
* [MySQL](https://www.mysql.com) - You can install it from https://www.mysql.com/downloads/.
* [Node.js](https://nodejs.org) - Install node.js from https://nodejs.org/es/download/. It's advisable to install the LTS version.

## General Installation instructions

You have to start creating a Google Client ID. Follow the instructions in the original project: https://www.sitepoint.com/google-auth-react-express/

The best option to start with this project is cloning it in your PC:

```
git clone https://github.com/tcrurav/ReactExpressGoogleLogin.git
```

This project contains 2 different parts:
* Frontend
* Backend

You need a node.js working environment. The LTS is recommended: https://nodejs.org/es/

Once you have cloned the project install all dependencies.

```
cd ReactExpressGoogleLogin/frontend
npm install

cd ReactExpressGoogleLogin/backend
npm install
```

* For your backend part:
1. You need a ReactExpressGoogleLogin/backend/.env file with a key for the JWT and Your Google Client ID:

```
GOOGLE_CLIENT_ID=Your google client id
JWT_SECRET=Your secret
```

* For your frontend part:
1. You need a ReactExpressGoogleLogin/frontend/.env file with Your Google Client ID:

```
REACT_APP_GOOGLE_CLIENT_ID=Your google client id
```

Finally to start enjoying this project.

```
cd ReactExpressGoogleLogin/backend
npm start

cd ReactExpressGoogleLogin/frontend
ionic serve
```

Enjoy!!!


## Built With

* [Visual Studio Code](https://code.visualstudio.com/) - The Editor used in this project
* [Node.js](https://nodejs.org/) - Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
* [express](https://expressjs.com/) - Fast, unopinionated, minimalist web framework for Node.js.
* [dotenv](https://www.npmjs.com/package/dotenv) - Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env. Storing configuration in the environment separate from code is based on The Twelve-Factor App methodology.

## Acknowledgments

* https://www.sitepoint.com/google-auth-react-express/. This project is just a copy of this project.
* https://openwebinars.net/blog/que-es-oauth2/. Interesting introduction to OAuth2.
* https://www.npmjs.com/package/google-auth-library. This is Google's officially supported node.js client library for using OAuth 2.0 authorization and authentication with Google APIs.
* https://medium.com/javarevisited/jwt-and-social-authentication-using-spring-boot-90e4faaa9204. JWT and Social Authentication using Spring Boot
* https://blog.prototypr.io/how-to-build-google-login-into-a-react-app-and-node-express-api-821d049ee670. How to build Google login into a React app and Node/Express API
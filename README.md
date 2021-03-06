# A Node/Express/Webpack Boilerplate

A comprehensive, configurable NodeJS/ExpressJS/Webpack server with options for ORMs for SQL/NoSQL databases and various user authentication, verification, and 2FA options.

To use, simply fork and clone the repo and edit config.js to your liking.
If either React, Angular, or Vue is to be used, check out the relevant branch.
Business logic is suggested to be implemented as modules in the ./lib folder.

## Protocol (select one)
- http
- https, with self-signed certs for use in development

## ORMs (configure one)
- Mongoose
- Sequelize

## Templating Engine (optional)
- Handlebars
- Suitable for use with any front-end framework (see section on other built-in features)

## User authentication options (configure any)
- Express-session
- Session-stored JSON web tokens
- Cookie-stored JSON web tokens
- PassportJS with JSON web tokens (for configuring an API server)
- PassportJS local authentication

## User verification options (optional)
- Email verification by nodemailer

## Two-Factor Authentication (optional)
- App-based authentication, e.g. Google/Microsoft Authenticator or Authy, using TOTP tokens

## Other built-in features
- AJAX form handling for single-page application building
- File uploads
- CSRF protection middleware
- Optional websockets readily setup for bi-directional server-client communication using socket.io. Turn this on in config.js.
- Unopinionated optional Webpack/Babel setup as express middleware. This avoids the need to run two servers concurrently (one for the front-end and one for express) and leaves your choice of front-end framework open. To use React, simply install the necessary npm packages and edit 'client-src/index.js'.
- Geolocation functions
- A JS utility library currently providing linked list implementation for your use

## Upcoming works
- Online payment systems


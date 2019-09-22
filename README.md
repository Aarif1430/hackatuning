A project by:

[Leonardo Motta](https://leomotta.me), [Adam Dias](https://github.com/adamdias), [Rafael Prado](https://rprado.myportfolio.com/)

# Hackatuning

Hey there, hackatuning is an open source hackathon management system.

## How to run the project

The project is a mono repository, you will need to run `yarn install` or `npm install` in both frontend and backend directory.

The frontend will need to know where to call the api, for that use the `API_URL` environment, and that is all, you may now run `yarn start` or `npm start`.

The backend will need more environment variables, `APP_URL` to know the url where the api is running, `WEB_URL` to know where our frontend is running, for cors proporse and the `NODE_ENV` which should be either production or development.

All routes will have a `v1` prefix eg. `http://localhost:3333/v1/route`.

To connect environment variables to connect to a SQL database with sequelize.

```js
DB_DIALECT=postgres
DB_HOST=
DB_USER=
DB_PASS=
DB_NAME=
```

To connect to MongoDB:

```js
MONGO_URL=
```

To connect to Redis database for background tasks such as sending emails.

```js
REDIS_HOST=127.0.0.1
REDIS_PORT=6379
```

To send emails via smtp with nodemailer, choose any smtp provider you want:

```js
MAIL_HOST=
MAIL_PORT=
MAIL_USER=
MAIL_PASS=
```

## MIT License

Copyright (c) 2019

[Leonardo Motta](https://leomotta.me), [Adam Dias](https://github.com/adamdias), [Rafael Prado](https://rprado.myportfolio.com/)

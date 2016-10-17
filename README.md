# Ikea Quiz Bot 

This is a simple quiz for Telegram. The rules of the game are pretty simple: bot gives you the name of the Ikea product and you need to guess what is this.

# Ikea quiz telegram bot 

This is a simple quiz for Telegram. The rules of the game are pretty simple: bot gives you the name of the Ikea product and you need to guess what is this.

## Run on your local machine

Create `.env` similar to `.env.example` file in the root folder with the following content:
```bash
NODE_ENV=debug
TOKEN=YOUR_TELEGRAM_BOT_TOKEN
MONGO=YOUR_MONGO_DB_CONNECTION_STRING
```
Then just run `npm`.

```bash
npm run start.debug
```

## Run on Heroku

Run following script within the Heroku CLI.

```bash
heroku config:set TOKEN=your_token --app your_app
heroku config:set MONGO=your_mongo_db --app your_app
heroku config:set NODE_ENV=production --app your_app
heroku config:set HEROKU_URL=$(heroku info --app your_app  -s | grep web-url | cut -d= -f2) --app your_app
```

Then just run `npm`.

```bash
npm run start
```

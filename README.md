# Simple Guys Bot

If you're as I am about the use of language in you Slack workspace, this will interest you.

With the existing [guys-bot-for-slack](https://glitch.com/~guys-bot-for-slack) needing some updates to work with the latest flavour of Slack API, I chose to recreate it using the most basic implementation of the Slack SDKs.

![Screenshot of the bot responding to the message](screenshot.png "Screenshot of the bot responding to the message")

The bot responds with an ephemeral message, not seen by anyone but the user who originally messaged.

It requires the bot be invited into the channels you want it to listen on, so it can be implemented by individuals, or teams, as channels require, if that is what you want.

## Installation

Get the repo.

```shell
git clone https://github.com/lukeocodes/guys-bot.git
cd guys-bot
```

Install it.

```shell
npm install
```

## Configuration

```shell
cp .env.example .env
```

Edit `.env` with your Slack Token (the Bot Access Token) and App Signing Secret, plus a URL for a document that explains your etiquette, inclusion, and diversity policy.

## Run Dev

```shell
npm run dev
```

## Run Prod

```shell
npm start
```
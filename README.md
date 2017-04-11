# toot

A simple command-line utility that allows you to post a "toot" (equivalent of a Tweet) on the Mastodon social network.

## Installation

    npm install -g toot

## Running first time

When you first run `toot` you will be asked some questions in order for *toot* to authenticate with your Mastondon service

    > toot
    Before you start using toot, you need to authenticate with your Mastodon server.
    ...

You will be asked for:

- which instance of Mastodon are you posting to? - there are [many](https://instances.mastodon.xyz/) e.g. toot.cafe
- what name you want to give your app? - the name you pick here will show up in your Mastodon settings under "Authorized apps"

You will then be asked to visit a long URL in your browser and be prompted for one further piece of information:

- the code displayed when you visit the URL?

This is a once-only operation. Then your configuration is saved (in `~/.mastodon.json`).

## Sending a toot

After the inital setup, sending a toot is a breeze:

    > toot "I'm sending a Toot from the command-line!"

## Why would I want this?

Perhaps you want to set up a Mastodon account for servers you are looking after. They can then be easily configured
to send status updates:
 
    > 
    > toot "$HOSTNAME is going down for maintenance. Farewell dear friends"
    > toot "$HOSTNAME is up. I'm back!"
 
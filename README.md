# screeps-bot-tooangel

[![CircleCI](https://circleci.com/gh/TooAngel/screeps.svg?style=svg)](https://circleci.com/gh/TooAngel/screeps)
[![npm version](https://badge.fury.io/js/screeps-bot-tooangel.svg)](https://badge.fury.io/js/screeps-bot-tooangel)
[![gitter](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/screeps-bot-tooangel/Lobby)

https://screeps.com/

## For in game room visitors:

Happy to see you visiting one of my rooms. [Visit FAQ to find answers](FAQ.md)

## Info

This is the AI I'm using for screeps. I managed to reach Top 10
from November 2015 - March 2016. Main Goal is to automate everything, no
manual interaction needed.

The AI is deployable on a private screeps server, follow the information on
[Steam](http://steamcommunity.com/sharedfiles/filedetails/?id=800902233).

## Note

This is not a good example for code quality or structure, most LOCs written
while fighting or other occasions which needed quick fixes or in the ingame
editor. But I think there are a couple of funny ideas. Every contribution is
welcome.

## Features

 - Automatic base building
 - External room harvesting
 - Basic mineral handling
 - Power harvesting
 - New rooms claiming on GCL level up
 - Automatic attack
 - Rebuild of fallen rooms

## Tweaking

Add a `src/friends.js` with player names to ignore them from all attack
considerations.

E.g.:
`module.exports = ['TooAngel'];`


Add a `src/config_local.js` to overwrite configuration values. Copy
`config_local.js.example` to `src/config_local.js` as an example. `src/config.js`
has the default values.

## Contributing

All kind of contribution is welcome, issues, contact via channels, pull requests.

Pull Request rule:
Prefix `[WIP]` in the PR title means, have a look if you like, but not ready to
merge.

## Upload

    npm install

    export email=EMAIL
    export password=PASSWORD

    grunt screeps

## Develop

    grunt jshint
    grunt jsbeautifier
    grunt jscs


## Design

[More details of the AI design](Design.md)

## Alliance

If you are playing on the live server with the TooAngel AI you are welcome
to join the [The Angels](Alliance.md) Alliance. Ping one of the members, you
can recognize us, because our rooms look like yours.

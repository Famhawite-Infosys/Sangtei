# Sangtei

<p align='center'>
  <a href="https://github.com/lalrochhara/Sangtei/actions/workflows/ci.yml"><img src="https://github.com/lalrochhara/Sangtei/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <a href="https://github.com/lalrochhara/Sangtei/actions/workflows/release.yml" alt="made-with-go"> <img src="https://github.com/lalrochhara/Sangtei/actions/workflows/release.yml/badge.svg" alt="Release"/> </a>
</p>


<p align='center'>
  <img src="https://img.shields.io/github/forks/lalrochhara/Sangtei?style=flat-square" alt="Forks">
  <img src="https://img.shields.io/github/stars/lalrochhara/Sangtei?style=flat-square" alt="Stars">
  <img src="https://img.shields.io/github/issues/lalrochhara/Sangtei?style=flat-square" alt="Issues">
  <img src="https://img.shields.io/github/license/lalrochhara/Sangtei?style=flat-square" alt="LICENSE">
  <img src="https://img.shields.io/github/contributors/lalrochhara/Sangtei?style=flat-square" alt="Contributors">
  <img src="https://img.shields.io/github/repo-size/lalrochhara/Sangtei?style=flat-square" alt="Repo Size">
  <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/lalrochhara/Sangtei&amp;title=Repo%20Views" alt="Views">
</p>

<p align='center'>
  <a href="https://go.dev/" alt="made-with-go"> <img src="https://img.shields.io/badge/Made%20with-Go-1f425f.svg?style=flat-square&logo=Go&color=blue" /> </a>
  <a href="https://deepsource.io/gh/lalrochhara/Sangtei/?ref=repository-badge"><img src="https://static.deepsource.io/deepsource-badge-light-mini.svg" alt="DeepSource"></a>
  <a href="https://makeapullrequest.com" alt="PRs Welcome"> <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" /> </a>
</p>

Sangtei is a Telegram Group managment bot made using **[Gotgbot](https://github.com/PaulSonOfLars/gotgbot)** and **[Go](https://go.dev)**, which makes it modern and faster than most of the exisitng Telegram Chat Managers.

**Sangtei's features over other bots:**
- Modern
- Fast
- Fully asynchronous
- Fully open-source
- Frequently updated
- Multi Language Support

Can be found on Telegram as [@Sangtei](https://t.me/dSangteiBot)
</br>

Sangtei is currently available in 1 Language as of now:
- **US English**

More languages can be managed in the _locales_ folder. Although we have added support for languages in bot, we still need contributors to translate the bot to other languages.

More langauges have been added to locales folder but need some configuration.

Help us bring more languages to the bot by contributing to the project on [Crowdin](https://crowdin.com/project/Sangteirobot)

## Requirements
- You need to have a *Mongo Database* (Cluster Preferred)
- You also need a *Redis Database* for caching (Required): Get a free redis database from [here](https://redis.com/try-free/)
- Linux/Windows machine (Ubuntu/Debain-based OS Preferred or Windows 10/Server2016 and later)

or
- Docker (Easiest way to setup the bot)

## How to setup

First Step!
- Star **⭐** the repository!!
- Fork **🔱** the repository before deploying and make changes in the fork.

It really motivates me to continue this project further.

### Deploy to Heroku
- Get your `API_ID` and `API_HASH` from [here](https://my.telegram.org/)
- Get your Bot Token from [@BotFather](https://t.me/BotFather)

**Note:** As it is banned with an unknown reason in heroku, follow the below steps carefully!
- First Fork this repo `:)`
- secondly, create an empty app in the Heroku, with a custom app name; and select Europe region for faster speed.
- Now go to the deploy tab of your app and under deployment method select GitHub and connect it.
- after that, type the forked repo name and select it now select main branch and enable auto deploy, at last click on deploy now button!
</h3>
<p align="center"><a href="https://heroku.com/deploy?template=https://github.com/lalrochhara/Sangtei"> <img src="https://img.shields.io/badge/Redirect%20To%20Heroku-black?style=for-the-badge&logo=heroku" width="200" height="35.45"/></a></p>

- Lastly, you must fill up all the vars in heroku (if using heroku) as directed in app.json file and now turn on the worker dyno to run it `:)`

**Must Add in heroku [config](https://dashboard.heroku.com/apps/yourappname/settings) :**
- `DB_URI` : Get one from [mongodb](https://cloud.mongodb.com/)
- `OWNER_ID` : your telegram id
- `MESSAGE_DUMP` : must be start with `-100` or your bot added in as **admin**
### Traditional

- Download a binary from [releases](https://github.com/lalrochhara/Sangtei/releases) page specific to your PC.
- Set the required env variables and run the binary

**Note:** Not a lot of people may be able to run using this because the instructions aren't clear but I'll try to make it clear in future.

### Docker

We currently publish a `ghcr.io/lalrochhara/Sangtei` Docker image based on alpine.

Set the Environmental vars using the `-e` flag in while running the container.

If all works well, bot should send message to the **MESSAGE_DUMP** Group!

### Other

You can download all binaries and release artifacts from the Releases page. Binaries are built for macOS, Linux, Windows, for amd64 and arm64 architectures.

If a binary does not yet exist for the OS/architecture you use, please open a GitHub Issue.


## Verify Signature

You can verify the integrity and authenticity of any released artifact using a public GPG key. All release artifacts are signed and have a corresponding signature file. Release artifacts are available on the Releases page.

# fetch GPG signing key
```bash
gpg --keyserver keyserver.ubuntu.com --recv 9CAFFF2AC5F94C7C
```
# example: verify a release package
```bash
gpg --verify Sangtei_2.0.1_darwin_amd64.tar.gz.sig Sangtei_2.0.1_darwin_amd64.tar.gz || echo "Verification failed!"
```

## Contributing to the project

- Make sure your PR works and doesn't break anything.
- You must join the support group [here](https://t.me/SangteiSupport).
- Make sure the CI passes.


## Special Thanks to
- [Paul Larsen](https://github.com/PaulSonOfLars) for his Original Marie Source Code and the amazing [Gotgbot](https://github.com/PaulSonOfLars/gotgbot) library.
- [ÁÑÑÍHÌLÅTØR SPÄRK](https://github.com/annihilatorrrr) always motivating me to make this project better.
- [jayantkageri](https://github.com/jayantkageri) for motivating me as well.
- [Anony](https://github.com/anonyindian) for helping me with bugs and issues in the project.
- Everyone else who inspired me to make this project, more names can be seen on commits!
- [DivideProjects](https://github.com/DivideProjects/Alita_Robot) We use some of  their Alita_Robot modules and copying their Docker Image Style.


### Copyright & License

* Copyright (C) 2020-2023 by [Nicky Lalrochhara](https://github.com/lalrochhara/Sangtei)
* Licensed under the terms of the [GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/lalrochhara/Sangtei/blob/master/LICENSE)
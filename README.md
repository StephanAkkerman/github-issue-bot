# Github Issue Discord Bot
This is a simple Python script for a Discord bot that can create GitHub issues through Discord commands.\
[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![MIT License](https://img.shields.io/github/license/StephanAkkerman/Issue_Bot.svg?color=brightgreen)](https://opensource.org/licenses/MIT)

---

## Setup
The first step is creating a Discord bot, setting up the basics, and inviting it to your server. For the first part you can watch this [video (watch until 2:20)](https://www.youtube.com/watch?v=Pbq7vPsHDtc).

Or follow these written instructions:
- Setup your own Discord bot, following this [written tutorial](https://realpython.com/how-to-make-a-discord-bot-python/) or this 
- Give the bot admin rights and all permissions possible, since this is the easiest way to set it up.
- Invite the bot to your server.
- Create the text channel where you would like to receive your Instagram updates in.

Last you need to fill in the important information in `config_example.yaml`, so the bot knows which server it should be connected to.
- Open `config.yaml` 
- Write your bot token behind `TOKEN:` (line 2)
- Write your server name behind `GUILD_NAME:` (line 3)
- Change the value behind `REPO:` (line 11)

## GitHub Token
To create a personal access token go to this [website](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) and follow the tutorial.
IMPORTANT: This bot needs no GitHub permissions so you can keep everything turned off in what you see at step 8.
After generating the token copy and paste it behind `TOKEN:` (line 10) in `config.yaml`. 

## GitHub Labels
This bot supports adding labels to new issues. However, your labels need to end with an emoji, below is an overview of the default labels we use:
- Bug 🐛
- Important ❗
- Improvement 📈
- Low priority 🥉
- Medium priority 🥈
- Top priority 🥇
- New feature ⭐
- Overhaul 🌈
- Text change ✍️

## Combining with your own bot
If you would like to combine this bot with your own bot, copy the `main.py` file and load your own Discord extenions. 
See line 31 in `main.py` on how to do this, or check out my other Discord bot for more extensive Discord bots and examples.

## Dependencies
The required packages to run this code can be found in the `requirements.txt` file. To run this file, execute the following code block:
```
$ pip install -r requirements.txt 
```
Alternatively, you can install the required packages manually like this:
```
$ pip install <package>
```

## How to run
- Clone the repository
- Fill in the fields in config.yaml
- Run `$ python src/main.py`
- Type `!issue` in your server
- See result

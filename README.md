[![Python 3.7](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-370/)
[![CodeQL](https://github.com/plasticuproject/pwnedBot/actions/workflows/codeql.yml/badge.svg)](https://github.com/plasticuproject/pwnedBot/actions/workflows/codeql.yml)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=plasticuproject_pwnedBot&metric=alert_status)](https://sonarcloud.io/dashboard?id=plasticuproject_pwnedBot)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=plasticuproject_pwnedBot&metric=security_rating)](https://sonarcloud.io/dashboard?id=plasticuproject_pwnedBot)
# pwnedBot
A  Discord bot implementation of Troy Hunt's haveibeenpwned.com service, <br />
a free resource for anyone to quickly assess if they may have been put <br />
at risk due to an online account of their's having been compromised or <br />
"pwned" in a data breach, using the hibpwned python library. <br />


## Prerequisites 
Head over to [DiscordApp](https://discordapp.com/developers/applications/me "DiscordApp") and create a new app. <br />
Record your *Client_ID*. On the left, click **Bot**, and then **Add Bot**. <br />
Once you are done setting up your bot, save your *Client_ID*, *Token*, and *Client Secret* in a safe place. <br />

Making calls to the haveibeenpwned API requires a key. You can purchase a HIBP-API-KEY
[here](https://haveibeenpwned.com/API/Key "HIBP-API-KEY"). <br />

##  Deployment (Tested with Python 3.7, 3.8+ May be borked)
```
git clone https://github.com/0xgingi/pwnedBot
cd pwnedBot
pip install -r requirements.txt
```

Create a .env file

```
HIBP_API_KEY=<your HIBP-API-KEY>
APP_NAME=<a unique app name for haveibeenpwned to recognize your app/bot>
DISCORD_TOKEN=<your discord bot TOKEN>
DISCORD_CLIENT_ID=<your discord CLIENT_ID>
BOT_PREFIX=<a prefix for your bot commands>
```
```
python pwned_bot.py
```

## Usage
To add bot to server add your *Client_ID* to this URL and visit in browser:  <br />
`https://discordapp.com/oauth2/authorize?client_id= <Client_ID> &scope=bot` <br />
When bot is active in server type "(prefix)help" for a list of commands.

![HELP](https://github.com/plasticuproject/pwnedBot/raw/master/images/help.png)
![BREACH_NAME](https://github.com/plasticuproject/pwnedBot/raw/master/images/breach_name.png)
![PASSWORD](https://github.com/plasticuproject/pwnedBot/raw/master/images/password.png)
![SEARCH](https://github.com/plasticuproject/pwnedBot/raw/master/images/search.png)
![PASTES](https://github.com/plasticuproject/pwnedBot/raw/master/images/pastes.png)
![PASTE_ID](https://github.com/plasticuproject/pwnedBot/raw/master/images/paste_id.png)

## License
All data sourced from https://haveibeenpwned.com <br />
Visit https://haveibeenpwned.com/API/v3 to read the Acceptable Use Policy <br />
for rules regarding acceptable usage of this API. <br />

This work is licensed under a [Creative Commons Attribution 4.0 International License.](https://creativecommons.org/licenses/by/4.0/) <br />
![CCv4](https://haveibeenpwned.com/Content/Images/CreativeCommons.png) <br />

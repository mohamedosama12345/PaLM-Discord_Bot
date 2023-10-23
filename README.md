# PaLM-Discord-Bot

Google PaLM API in Discord.

## Notice

Discord only can handle 2000 characters per message, so I manually set the PaLM can only outputting no more than 145 tokens. If your channel can handle 4000 or even more, make the `output_token_limit= 145` in `main.py` value doubled or more.


## Example:
Casual Chatting:

![](https://github.com/mohamedosama12345/PaLM-Discord_Bot/blob/main/images/image_1.png)

Coding:

![Coding](https://github.com/mohamedosama12345/PaLM-Discord_Bot/blob/main/images/image_2.png)

## Command

`/palm` to chat with PaLM.

## Installation

### Get your Discord API

1. Go [Discord Dev](https://discord.com/developers/applications)
2. Go `Application` on the left part
3. Go `New Application`, create a new Bot
4. Go `Bot` on the left
5. Click `Add bot`
6. Turn on `MESSAGE CONTENT INTENT`
7. `Save Change`
8. View and save your API Key on the top of page `View Token`, or reset one if you don't remember
9. Click OAuth2 on the left part
10. Click on `URL Generator`
11. Choose `bot` in `SCOPES`, `Administrator` in `BOT PERMISSIONS`
12. Copy the link at bottom into your browser, add bot and authorize to you server.
### Get your PaLM API
Go to [MakerSuite](https://makersuite.google.com/app/apikey), and create an API key for this application.
### Deploy on your machine
1. git clone this repository
2. `pip install discord google-generativeai`
3. `cd PaLM-Discord-Bot`
4. `notepad main.py`
5. replace with your Discord API Key and PaLM API Key at following lines: 
    `palm.configure(api_key = "PaLM_API_KEY")`
    `client.run("DISCORD_TOKEN")`
6. `python main.py`


## Reference: 

https://discordpy.readthedocs.io/en/stable/#getting-started

https://developers.generativeai.google/api/python/google/generativeai
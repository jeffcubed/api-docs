# /bots

`GET /bots` or `GET /bots?key=value`  
Returns an array of [bot objects](/models/Bot.md) (matching the given URL parameters)

---

:lock: `POST /bots`  
Creates a new bot listing  
Returns an array filled with the created bot  
Parameters:  

| Key               | Type    | Description                                           | Example                                                                                        |
|-------------------|---------|-------------------------------------------------------|------------------------------------------------------------------------------------------------|
| discord_id        | STRING  | Discord's snowflake for the bot account               | "277411860125581312"                                                                           |
| short_description | STRING  | A short description of the bot                        | "A meme bot"                                                                                   |
| long_description  | STRING  | A long description of the bot                         | "This bot has a lot of features, like memes, memes and.. memes!"                               |
| invite_url        | ?STRING | A custom invite URL for the bot (optional)            | "https://discordapp.com/oauth2/authorize?client_id=277411860125581312&scope=bot&permissions=8" |
| website_url       | ?STRING | A URL pointing to the bot's website (optional)        | "https://fbot.menchez.me/"                                                                     |
| repo_url          | ?STRING | A URL pointing to the bot's Git repository (optional) | "https://github.com/xmatmen/fbot"                                                              |
| library           | ?STRING | The library the bot is written in                     | "discord.js"                                                                                   |
| help_command      | STRING  | The bot's help command                                | "f!help"                                                                                       |

---

`GET /bots/:id`  
Returns an array filled with a single bot object matching the ID

---

:lock: `PUT /bots/:id`  
Modifies the given bot listing  
Returns the updated bot model  
Parameters:

| Key               | Type    | Description                                           | Example                                                                                        |
|-------------------|---------|-------------------------------------------------------|------------------------------------------------------------------------------------------------|
| short_description | STRING  | A short description of the bot                        | "A meme bot"                                                                                   |
| long_description  | STRING  | A long description of the bot                         | "This bot has a lot of features, like memes, memes and.. memes!"                               |
| invite_url        | ?STRING | A custom invite URL for the bot (optional)            | "https://discordapp.com/oauth2/authorize?client_id=277411860125581312&scope=bot&permissions=8" |
| website_url       | ?STRING | A URL pointing to the bot's website (optional)        | "https://fbot.menchez.me/"                                                                     |
| repo_url          | ?STRING | A URL pointing to the bot's Git repository (optional) | "https://github.com/xmatmen/fbot"                                                              |
| library           | ?STRING | The library the bot is written in                     | "discord.js"                                                                                   |
| help_command      | STRING  | The bot's help command                                | "f!help"                                                                                       |
| active            | BOOLEAN | Wether this bot has been approved (Mod only)          | true                                                                                           |
| spotlight         | BOOLEAN | Wether this bot is in a spotlight (Mod only)          | false                                                                                          |

---

:lock: `DELETE /bots/:id`  
Deletes the given bot listing
Returns the deleted bot's data

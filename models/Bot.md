# Bot

```js
{
  id: INTEGER,  // The internal bot ID
  user: USER, // The user that submitted this bot (A user object, see the docs for help)
  name: STRING,
  discord_id: STRING, // Discord's Bot ID / Snowflake
  short_description: STRING,
  long_description: STRING,
  avatar_url: STRING,
  website_url: STRING | null,
  repo_url: STRING | null,
  help_command: STRING,
  library: STRING | null,
  spotlight: BOOLEAN, // Wether this bot is advertised/pinned
  active: BOOLEAN, // Wether this bot has been approved by modearators
  created_at: STRING,
  updated_at: STRING
}
```

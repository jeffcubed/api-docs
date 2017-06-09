# Bot

```js
{
  id: INTEGER,  // The internal bot ID
  user: USER, // A user object, see the docs for help
  name: STRING,
  discord_id: STRING, // Discord's Bot ID / Snowflake
  short_description: STRING,
  long_description: STRING,
  avatar_url: STRING,
  website_url: STRING,  // Optional
  repo_url: STRING, // Optional
  help_command: STRING,
  library: STRING,  // Optional
  spotlight: BOOLEAN, // Wether this bot is in a spotlight, aka advertised/pinned
  active: BOOLEAN, // Wether this bot has been checked by admins
  created_at: STRING,
  updated_at: STRING
}
```

# NadekoBot Migration Helper

[NadekoBot is a discord bot which enables gamification and interactivity in your discord server.](https://nadeko.bot/)

Recenly I faced issues with my NadekoBot and I found out that auto update no longer worked because the project switched from GitHub to GitLab. Meanwhile a lot changed and upgrade to newer versions no longer worked. I needed a data migration.

I wrote this migration helper to migrate the data from the sqlite database of the old bot to the new bot. For me it worked and I could run my new NadekoBot with my existing data.

Important Note: The helper is most probably incomplete for your case. You might need to select also other tables. Since I did not use all functionalities of NadekoBot, only a portion of tables was sufficient to make the migration successful. Still this script provides a good starting point, if you are also facing upgrade issues.

## Dependencies
* sqlite3

## Quickstart
* place your old NadekoBot sqlite database into the "old" folder
* place your new NadekoBot sqlite database into the "new" folder
* update and run notebook according to your needs
 
 Warning: Make sufficient backups. The database in the "new" folder gets overwritten with the old data.

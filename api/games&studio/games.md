## All game's info
### Default information
**https://playvortex.io/api/games** \
Request method`GET`
```
[{"id":1,"name":"Demo","description":"Test physics and features while developing Vortex.","creator_id":1,"creator_name":"TheHaloDeveloper","thumbnail_version":"a10c9ec0","player_count":6},{"id":3,"name":"Snowy Peak","description":"it's really chilly up here","creator_id":2,"creator_name":"kostas","thumbnail_version":"6087342e","player_count":0},{"id":4,"name":"The Crossbridges","description":"A Large island located in the Vortexic Ocean, divided into 4 slices and connected by colorful bridges. Which path will you choose?","creator_id":3135,"creator_name":"Eduardo","thumbnail_version":"bf381df7","player_count":0}]
```
id`The Unique ID of the game`\
name`The name of the game`\
description`The description of the game`\
creator_id`The UUID of the game's creator`\
creator_name`The username of the game's creator`\
thumbnail_version`The thumbnail's version (Used for the thumbnail image)`\
player_count`The live ccu count`

### Additional information
**https://playvortex.io/api/game-stats** \
Request method`GET`

Example api response:
```
{"1":{"active":0,"visits":95811},"2":{"active":0,"visits":19302},"3":{"active":0,"visits":37428},"4":{"active":0,"visits":36435},"5":{"active":0,"visits":19128},"6":{"active":0,"visits":17420},"7":{"active":1,"visits":20928},"8":{"active":0,"visits":174747}}
```
active`The live ccu count`
visits`Total visits count`
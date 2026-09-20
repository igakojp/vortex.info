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

---

### Game thumbnails

**https://playvortex.io/assets/thumbnails/{game_id}?v={thumbnail_version}** \
Request method`GET` (just an image link) \
*(You don't need to have the `?v={thumbnail_version}` part if you just want the latest version.)*

Example result (gameid: 8 thumbnail_version: latest)
<img src="https://playvortex.io/assets/thumbnails/8" />

---
### More in-depth game info
**https://playvortex.io/api/games/{game_id}** \
Request method`GET`
```
{"id":8,"name":"Vortexia","description":"A small little town to hangout with others! ","creator_id":2705,"creator_name":"yea","thumbnail_version":"07781601","player_count":1,"instances":[{"instance_id":0,"players":1,"user_ids":[42382]}],"total_instances":1,"has_more":false}
```
id`The game Unique ID` (This is the same result to [this](#default-information)) \
name`The name of the game` (This is the same result to [this](#default-information)) \
description`The description of the game` (This is the same result to [this](#default-information)) \
creator_id`The UUID of the game creator` (This is the same result to [this](#default-information)) \
creator_name`` (This is the same result to [this](#default-information)) \
thumbnail_version`The version of the thumbnail` (This is the same result to [this](#default-information)) \
player_count`The full player count` (This is the same result to [this](#default-information)) \
instances`` \
    instance_id`The id of this instance` \
    players`The amount of players in this one instance` \
    user_ids:[first_user_id, second_user_id, third_user_id, ...]`The first 6 users that are in this server` \
    <img src="https://raw.githubusercontent.com/igakojp/vortex.info/refs/heads/main/images%26videos/image.png" alt="Vortex Logo" style="display:inline; vertical-align:middle;" width="100"> \
total_instances
has_more

### Additional information
**https://playvortex.io/api/game-stats** \
Request method`GET`

Example api response:
```
{"1":{"active":0,"visits":95811},"2":{"active":0,"visits":19302},"3":{"active":0,"visits":37428},"4":{"active":0,"visits":36435},"5":{"active":0,"visits":19128},"6":{"active":0,"visits":17420},"7":{"active":1,"visits":20928},"8":{"active":0,"visits":174747}}
```
active`The live ccu count`
visits`Total visits count`

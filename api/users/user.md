## Basic user information
**https://playvortex.io/api/users/{user_id}** \
Request method`GET`
```
{"id":1,"username":"TheHaloDeveloper","bio":"hey im halo this is my bio i hope you have a nice time on Vortex bye guys :)","friend_count":37,"follower_count":3786,"following_count":14,"visits":115425,"friendship_status":"request_sent","follow_status":"following","online_status":"offline","created_at":"2026-04-23T05:37:25.988850+00:00","is_deleted":false,"is_staff":true,"is_moderator":true,"is_booster":true,"is_content_creator":true,"shirt_id":4,"last_seen":"2026-09-19T17:39:29.588121+00:00"}
```
id`The UUID(Unique user ID)` \
username`The Unique username of the user` \
bio`The about me section of the user (Can break lines using \n\n)` \
friend_count`The amount of friends that the user has` \
follower_count`The amount of followers that the user has` \
following_count`The amount users this user follows` \
visits`The total visits on all of the games the user published` \
friendship_status`friends/none (Only for yourself, self)` \
follow_status`not_following/following (Only for yourself, self)` \
online_status`offline/online/in_game/in_studio` \
created_at`The exact time of the account creation time (ISO 8601 date-time with a UTC offset)` \
is_deleted`If the account is banned, or deleted (uses boolean)` \
is_staff`If the user is apart of the staff team (uses boolean)` \
is_moderator`If the user is apart of the moderator team (uses boolean)` \
is_booster`If the user boosts the official Vortex Discord server (uses boolean)` \
is_content_creator`If the user is a content creator in any platform` \
shirt_id`The id of the shirts worn. (Only the shirt exists)` \
last_seen`The last time the user was online (ISO 8601 date-time with a UTC offset)` (This might be a bad idea of making it so that anyone without an account can even see this part)
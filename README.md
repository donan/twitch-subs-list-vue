# twitch-subs-list-vue
####List your twitch subs

#####Author: Pablo CL
#####Website: [se32.com](http://www.se32.com)
***

##How to use it:

1 Create an APP on https://dev.twitch.tv/ and obtain your APP Client_ID
2 Send an authorization request to the twitch API using your Client_ID
` https://id.twitch.tv/oauth2/authorize?response_type=token&client_id=XXXXXXXX&redirect_uri=http://localhost&scope=channel:read:subscriptions `
3 Store somewhere the access_token value from the response
4 Load this website using your client_id, the token as the "auth" value and your login username as the value of "login"
` https://mywebsite.com/?client_id=ZZZZ&auth=XXXXXXXX&login=YYYYYYYY `

TODO: Fix request rate and handle pagination.

***
##Query string parameters:
*  **client_id** - Your APP Client_ID.
*  **auth** - Your Twitch Access Token.
*  **login** - Twitch login username.
*  **icons** - 0 or 1 to show/hide the icons of the type of sub.
*  **style** - change the theme, values: default, white, twitch.

Example using all the parameters:
` https://mywebsite.com/?client_id=ZZZZ&auth=XXXXXXXX&login=YYYYYYYY&icons=1&style=twitch`

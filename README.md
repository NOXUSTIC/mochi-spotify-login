# Mochi Spotify login

Spotify only sends logins back to https pages, but a Mochi robot serves its app over plain http on your WiFi.
This one-file page receives the login from Spotify and hands the one-time code back to the Mochi app on your
own network (it only forwards to local addresses such as 192.168.x.x or name.local). It stores nothing, and the
code is useless without a secret that never leaves the robot's page (PKCE).

Use `https://noxustic.github.io/mochi-spotify-login/` as the Redirect URI of the Spotify app.

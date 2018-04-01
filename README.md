## shpotify-get-playlists

This fetches all of your Spotify playlists as individual JSON files.

To get started, get set up with the Spotify API.
For details: https://developer.spotify.com/web-api/tutorial/

Store your Spotify Client ID in the file `~/config/shpotify/.env.d/SPOTIFY_CLIENT_ID`.
Store your Spotify Client Secret in the file `~/config/shpotify/.env.d/SPOTIFY_CLIENT_SECRET`.
Store your Spotify Refresh Token in `~/config/shpotify/.env.d/SPOTIFY_REFRESH_TOKEN`.
Store your Spotify Access Token in `~/config/shpotify/.env.d/SPOTIFY_ACCESS_TOKEN`.

Your access token will expire in about an hour.
Use the `./shpotify-refresh-token` script when you need a new one.
It will fetch a fresh token and store it in `~/config/shpotify/.env.d/SPOTIFY_ACCESS_TOKEN`.

Running `get-playlists` will create one JSON file for each of your playlists,
both your own and any you follow, with all track metadata available under
`~/Code/spotify/playlists`. Create this directory beforehand.

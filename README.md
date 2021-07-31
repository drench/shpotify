## shpotify

This is a command line interface to the Spotify API, written in `zsh`.
It also requires `jq` and `curl` which you may need to install yourself.

To get started, get set up with the Spotify API.
For details: https://developer.spotify.com/web-api/tutorial/

Store your Spotify Client ID in the file `~/config/shpotify/.env.d/SPOTIFY_CLIENT_ID`.
Store your Spotify Client Secret in the file `~/config/shpotify/.env.d/SPOTIFY_CLIENT_SECRET`.
Store your Spotify Refresh Token in `~/config/shpotify/.env.d/SPOTIFY_REFRESH_TOKEN`.
Store your Spotify Access Token in `~/config/shpotify/.env.d/SPOTIFY_ACCESS_TOKEN`.

Your access token will expire in about an hour but `shpotify` will automatically
refresh it if it's nearing or past expiration.


### Running it

Clone this repo and `cd` into it.
Load the `zsh` completion:

```shell
eval "$(./shpotify --completion-code)"
```

Type `./shpotify` and hit your "tab" key to see what's available.

This is a very incomplete implementation of the API.
If `zsh` tab completion exists for it, consider it supported.

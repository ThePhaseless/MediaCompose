# MediaCompose

A docker-compose project for fast self-hosted media center

## How to use

Set envs in `env.env` file or in any other way and
**_drop insides of Config file inside CONFIG_PATH!_**

### Security Info

API keys are the same every for everyone who use this repo, so it's not recommended to use outside of your local network. If you want to do so, i recommend resetting every API key in every app and updating them in appropriate settings.

To run with .env file use command next in folder with `docker-compose.yml`:

`sudo docker-compose --env-file env.env up -d`

### Credentials:

_I recommend changing them as soon as possible_

- login: `admin`

- password: `admin`

## Docker images

This docker-compose file will download:

- Jellyfin

- Jellyseer

- Sonarr

- Radarr

- qBittorrent

- Prowlarr

- Bazarr

- Httpd (for your main side, no files)

- watchtower

- File Browser

## What I've done:

- Synced Sonarr, Radarr, Bazarr, Prowlarr with qBittorrent

- Jellyfin grabs releases automatically from MEDIA_PATH

- Jellyfin configured to use Intel Hardware Transcoding (double check if that works for you)

- Synced Jellyseer with Jellyfin

- Config, Media and home paths preadded to File Browser

# Please, don't trust me with my settings, check every one of them and verify that they fit your needs!

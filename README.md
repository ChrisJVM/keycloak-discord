# keycloak-discord

Keycloak Social Login extension for Discord.

## Changes

I forked this repo from [Andy Thorne](https://github.com/andythorne) to add in his updated fix for keycloak 25.x. I plan
 on maintaining this fork specifically for my projects and will update it as needed. As such, the versioning for this 
project will change to reflect it as mine, but it was originally based on version 0.5.1-SNAPSHOT.

I've updated the pull for the username to remove discords discriminator and added a pull for the users discord id and 
avatar hash.

## Install

Download `keycloak-discord-<version>.jar` from [Releases page](https://github.com/ChrisJVM/keycloak-discord/releases).
Then deploy it into `$KEYCLOAK_HOME/providers` directory.

## Setup

### Discord

Access to [Discord Developer Portal](https://discord.com/developers/applications) and create your application.
You can get Client ID and Client Secret from the created application.

### Keycloak

Note: You don't need to setup the theme in `master` realm from v0.3.0.

1. Add `discord` Identity Provider in the realm which you want to configure.
2. In the `discord` identity provider page, set `Client Id` and `Client Secret`.
3. (Optional) Set Guild Id(s) to allow federation if you want.


## Source Build

Clone this repository and run `mvn package`.
You can see `keycloak-discord-<version>.jar` under `target` directory.


## Licence

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)


## Author

- [Hiroyuki Wada](https://github.com/wadahiro)


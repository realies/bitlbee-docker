## BitlBee on Alpine with Plugins
![Docker Pulls](https://img.shields.io/docker/pulls/vanityshed/bitlbee-alpine-plugins.svg)
![Docker Stars](https://img.shields.io/docker/stars/vanityshed/bitlbee-alpine-plugins.svg)

Minimal build of latest BitlBee on latest Alpine with latest plugins for:

| Plugin | Protocol | Version | Commit |
|:-------|:---------|:--------|:-------|
| [bitlbee-discord](https://github.com/sm00th/bitlbee-discord) | discord | 0.4.1 | [3e7c694](https://github.com/sm00th/bitlbee-discord/commit/3e7c694bf989cc523f003d77e62f840841bf86ec) |
| [bitlbee-steam](https://github.com/bitlbee/bitlbee-steam) | steam | 1.4.2 | [a6444d2](https://github.com/bitlbee/bitlbee-steam/commit/a6444d216c0ec4c9038b7b74b00c93ebbb99a2f4) |
| [bitlbee-facebook](https://github.com/jgeboski/bitlbee-facebook) | facebook | 1.1.2 | [553593d](https://github.com/bitlbee/bitlbee-facebook/commit/553593d07170d6d1563d0079dbedd481dcec5b00) |
| [libpurple](https://pkgs.alpinelinux.org/package/v3.8/community/x86_64/libpurple) | gg, irc, novell, simple, zephyr | 2.13.0 | [235ba2b](https://git.alpinelinux.org/cgit/aports/commit/?id=235ba2b3a865227ff7252005fbf5ca0686949edb) |
| [libpurple-bonjour](https://pkgs.alpinelinux.org/package/v3.8/community/x86_64/libpurple-bonjour) | bonjour | 2.13.0 | [235ba2b](http://git.alpinelinux.org/cgit/aports/commit/?id=235ba2b3a865227ff7252005fbf5ca0686949edb) |
| [libpurple-oscar](https://pkgs.alpinelinux.org/package/v3.8/community/x86_64/libpurple-oscar) | aim, icq, oscar | 2.13.0 | [235ba2b](http://git.alpinelinux.org/cgit/aports/commit/?id=235ba2b3a865227ff7252005fbf5ca0686949edb) |
| [libpurple-xmpp](https://pkgs.alpinelinux.org/package/v3.8/community/x86_64/libpurple-xmpp) | jabber, xmpp | 2.13.0 | [235ba2b](http://git.alpinelinux.org/cgit/aports/commit/?id=235ba2b3a865227ff7252005fbf5ca0686949edb) |
| [skype4pidgin](https://github.com/EionRobb/skype4pidgin) | skype | 1.5 | [2290013](https://github.com/EionRobb/skype4pidgin/commit/229001358707089bbe0982646f5bcde73ca92ece) |
| [slack-libpurple](https://github.com/dylex/slack-libpurple) | slack | 0.1 | [ee0f2bd](https://github.com/dylex/slack-libpurple/commit/ee0f2bd49e526a38525eadd6fbdf27e9488719f0) |
| [telegram-purple](https://github.com/majn/telegram-purple) | telegram | 1.3.1 | [f686f8a](https://github.com/majn/telegram-purple/commit/f686f8a6e7669bce2e50645638497abfc3d6a8ef) |

## Typical Usage

For configuration persistance, `/opt/dockerdata/bitlbee` should be present on the host with sufficient permissions.

##### Using Docker CLI
```
docker run -d --name bitlbee --restart=always \
-v /opt/dockerdata/bitlbee:/bitlbee-data:rw \
-v /etc/localtime:/etc/localtime:ro \
-p 6667:6667 \
vanityshed/bitlbee-alpine-plugins
```

##### Using Docker Compose
```
docker-compose up -d
```

## BitlBee on Alpine Edge with Plugins

Minimal build of latest BitlBee on latest Alpine with latest plugins

| Package | Protocol | Version | Commit |
|:--------|:---------|:--------|:-------|
| [bitlbee](https://github.com/bitlbee/bitlbee) | irc, jabber, twitter | 3.6 | [e979b0f](https://github.com/bitlbee/bitlbee/commit/e979b0f3ed6aee99debe6e1ce1038da7c6d57920) |
| [bitlbee-discord](https://github.com/sm00th/bitlbee-discord) | discord | 0.4.3 | [9466079](https://github.com/sm00th/bitlbee-discord/commit/9466079361c49639cef7cc2eb54dba94544be307) |
| [bitlbee-steam](https://github.com/bitlbee/bitlbee-steam) | steam | 1.4.2 | [a6444d2](https://github.com/bitlbee/bitlbee-steam/commit/a6444d216c0ec4c9038b7b74b00c93ebbb99a2f4) |
| [bitlbee-facebook](https://github.com/jgeboski/bitlbee-facebook) | facebook | 1.2.0 | [c76b36b](https://github.com/bitlbee/bitlbee-facebook/commit/c76b36bd29ee8b32fd038c7b7254931c71ecce1b) |
| [libpurple](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple) | gg, irc, novell, simple, zephyr | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [libpurple-bonjour](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple-bonjour) | bonjour | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [libpurple-oscar](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple-oscar) | aim, icq, oscar | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [libpurple-xmpp](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple-xmpp) | jabber, xmpp | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [purple-instagram](https://github.com/EionRobb/purple-instagram) | instagram | git-HEAD | [420cef4](https://github.com/EionRobb/purple-instagram/commit/420cef45db2398739ac19c93640e6fff42865bb1) |
| [skype4pidgin](https://github.com/EionRobb/skype4pidgin) | skype | 1.5 | [cf65095](https://github.com/EionRobb/skype4pidgin/commit/cf650950f937cf4faf834063128693a6c6a30a00) |
| [slack-libpurple](https://github.com/dylex/slack-libpurple) | slack | git-HEAD | [7f61c84](https://github.com/dylex/slack-libpurple/commit/7f61c842e33202170fcd77209c8d4bded09703b0) |
| [telegram-purple](https://github.com/majn/telegram-purple) | telegram | 1.4.3 | [ca42dcf](https://github.com/majn/telegram-purple/commit/ca42dcf0e6bebe2d0f818e1221db9518561dd8a0) |

## Typical Usage

##### Using Docker CLI
```
docker run -d --name bitlbee --restart=unless-stopped \
-v /persistent/appdata:/bitlbee-data \
-p 6667:6667 \
realies/bitlbee
```

##### Using Docker Compose
```
docker-compose up -d
```


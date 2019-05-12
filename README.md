## BitlBee on Alpine Edge with Plugins

Minimal build of latest BitlBee on latest Alpine with latest plugins.

| Package | Protocol | Version | Commit |
|:--------|:---------|:--------|:-------|
| [bitlbee](https://github.com/bitlbee/bitlbee) | irc | 3.5.1 | [fe122f3](https://github.com/bitlbee/bitlbee/commit/fe122f3fa913c5bbb64f8d815b4687df44c5d422) |
| [bitlbee-discord](https://github.com/sm00th/bitlbee-discord) | discord | 0.4.2 | [aa0bbf2](https://github.com/sm00th/bitlbee-discord/commit/aa0bbf2df851b1fd1b27164713121d20c610b7c5) |
| [bitlbee-steam](https://github.com/bitlbee/bitlbee-steam) | steam | 1.4.2 | [a6444d2](https://github.com/bitlbee/bitlbee-steam/commit/a6444d216c0ec4c9038b7b74b00c93ebbb99a2f4) |
| [bitlbee-facebook](https://github.com/jgeboski/bitlbee-facebook) | facebook | 1.2.0 | [c76b36b](https://github.com/bitlbee/bitlbee-facebook/commit/c76b36bd29ee8b32fd038c7b7254931c71ecce1b) |
| [libpurple](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple) | gg, irc, novell, simple, zephyr | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [libpurple-bonjour](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple-bonjour) | bonjour | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [libpurple-oscar](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple-oscar) | aim, icq, oscar | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [libpurple-xmpp](https://pkgs.alpinelinux.org/package/edge/community/x86_64/libpurple-xmpp) | jabber, xmpp | 2.13.0-r2 | [38d8a7c](http://git.alpinelinux.org/cgit/aports/commit/?id=38d8a7c2ca995bf1fc1c310303941fcad35ae429) |
| [skype4pidgin](https://github.com/EionRobb/skype4pidgin) | skype | 1.5 | [14f1b69](https://github.com/EionRobb/skype4pidgin/commit/14f1b69b6292bbdc98cca484b050ec8359394c4e) |
| [slack-libpurple](https://github.com/dylex/slack-libpurple) | slack | 0.1 | [c10cc72](https://github.com/dylex/slack-libpurple/commit/c10cc72e441b3edbeee5b00049a4a1c977d746e6) |
| [telegram-purple](https://github.com/majn/telegram-purple) | telegram | 1.4.1 | [9ba0e57](https://github.com/majn/telegram-purple/commit/9ba0e5702d0c17f93e7830bc35cba331f90583ba) |

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


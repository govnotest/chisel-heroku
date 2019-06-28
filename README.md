chisel-heroku
=============

Deploy [chisel](https://github.com/jpillora/chisel) to [Heroku](https://www.heroku.com/) as a [SOCKS5](https://en.wikipedia.org/wiki/SOCKS) proxy.

### Getting started

heroku container:login

heroku config:set CHISEL_AUTH=user:pass -a your-app-name

heroku container:push web -a your-app-name

heroku container:release web -a your-app-name


Connect your chisel client:
chisel client --auth user:pass https://your-app-name.herokuapp.com socks

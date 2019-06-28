chisel-heroku
=============

### Getting started

create app in heroku dashboard


on PC:

git clone https://github.com/govnotest/chisel-heroku.git

cd chisel-heroku/

heroku container:login

heroku config:set CHISEL_AUTH=user:pass -a your-app-name

heroku container:push web -a your-app-name

heroku container:release web -a your-app-name


Connect your chisel client:
chisel client --auth user:pass https://your-app-name.herokuapp.com socks

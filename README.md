Xernion is nginx config inside docker originally to make reversing proxy for medium custom domain purpose,
but you can change to your specified domain to!

See my [example](http://wlab.me:9999)

### What this things can do
- Making custom domain on medium for free :3, as you know we need to pay $75 for custom domain, this is my first intention to make this repo
- Modify it and you can make your own proxy server!

### Need to improved
- XHR rejected :(
- some link that refer to medium member and article, also image didnt load.

### Prerequisite
- docker
- docker-compose
- eagerness to learn and facing some errors :3

### How to run locally or in server

modify url resource and proxy as nginx doesnt support dynamic variable

for example i use this link for source

https://medium.com/dev-channel/

and this link for proxy

http://rizki.wlab.me

just type ```docker-compose up```

and by default this will run in port 9999

### Gitlab CI Config

you need to specify these variable in gitlab environment variable
- APP_DIR = location of your app
- GIT_ORIGIN = git url ssh access to your repository
- SSH_HOST = server location
- SSH_USER = your user to access ssh
- SSH_PASSWORD = your user password to access ssh
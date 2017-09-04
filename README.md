# node-certbot
A NodeJS mini-server to generate SSL Certificates in Webroot mode with Certbot

## install node server
```
npm install
node renew-srv.js
(or pm2 start renew-srv.js)

# ensure webroot method works for certbot :
curl http://example.com/.well-known/acme-challenge/9001
```

## install certbot
```
wget https://dl.eff.org/certbot-auto
chmod a+x certbot-auto

./certbot-auto certonly --webroot
./certbot-auto renew --dry-run
./certbot-auto renew

```
## usefull links
[Certbot installation method for Debian 7 Wheezy](https://certbot.eff.org/#debianwheezy-other)  
[Using Let's Encrypt with Express](https://medium.com/@yash.kulshrestha/using-lets-encrypt-with-express-e069c7abe625)  
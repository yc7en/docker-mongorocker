docker-mongorocker fork
=======================

Just the original docker with some features for customization.

Instructions:
 - Link to a MongoDB container and name the link "mongo" in this side.
 - Expose mongorock port 80 (ie, in port 8080)

```bash
    docker run ... -l mymongocontainername:mongo -p 8080:80
```

Notes:
 - rockmongo user/pass: admin (no password) !!!!!!!!!!!!! BE CAREFUL !!!!!!!!!!!!!!
 - MongoDB user/pass: no pass (so nothing configured in config.php)



You can also define a hostname "rockmongo.docker.local" to your docker IP (localhost, boot2docker IP, panamax IP...) to access rockmongo's nginx.

 - You can also use "docker run" env params to change:
  - Name of linked MongoDB
  - MongoDB hostname, MongoDB port (by default: linked MongoDB hostname autoset by docker & 27017)
  - Different hostname for nginx site

# Wordpress

This is just a bog-standard config for setting up a wordpress site!



## Usage

Run:

```bash
docker compose up
```



Then go to [http://localhost:5555](http://localhost:5555) to finalize setup!



## Things to change for prod

By default the port mapping is 5555:80 in `compose.yaml`, if you want to go live with this you should change this to 80:80



**EVERY PASSWORD IS BAD**, change all of them in `compose.yaml`



**DEPENDENCIES ARE PINNED**, check if there are new versions of mariaDB/mysql and use those if you can!

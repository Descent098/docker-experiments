# Apache/php

This project seeks to give you a quick way to setup PHP with apache as the HTTP server.

By default this maps to the **host port** 4040 to avoid common port conflicts. This is defined in `compose.yaml` and should be changed to 80:80 if you want to expose this publicly.



## Usage

Run:

```bash
docker compose up
```

and then navigate to [http://localhost:4040](http://localhost:4040)

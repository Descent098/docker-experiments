# Leantime

[Leantime](https://leantime.io/) is a system for project planning, similar to JIRA. 



You can find the docker from-scratch [official repo here](https://github.com/Leantime/docker-leantime), and the [source code here](https://github.com/Leantime/leantime).



This repo is a fully batteries-included version that has a built in mysql in the docker compose. This repo has **no affiliation with the maintainers of leantime**.



## Usage

Create your docker network first:

```bash
docker network create leantime-net
```

Then bring up the app using:

```bash
docker compose up
```

From there you will be able to access the application at [http://localhost:5050](http://localhost:5050)



For more details check out the [leantime documetnation](https://docs.leantime.io/)



## Security & Production

The default values in the `docker-compose.yml` are trash and insecure. **DO NOT USE THEM**, when/if you want to push to production change these to real passwords and not these defaults.
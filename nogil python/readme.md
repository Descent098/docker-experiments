# No-GIL Python

This project is a simple docker template (using flask) to use [Sam Gross' Gil-less fork of python](https://github.com/colesbury/nogil).

You can see details about this system, and why it's interesting in his [2022 pycon talk](https://www.youtube.com/watch?v=EZCtpnc0IJA&t=2082s)

## Usage

With docker running, simply run `docker compose up`, and from there it maps port 8080 and exposes it. You can then access the file at [http://localhost:8080/](http://localhost:8080/)

If you want to change the entrypoint to a new file (instead of `routes.py`) then go into the Dockerfile and change the last RUN command.


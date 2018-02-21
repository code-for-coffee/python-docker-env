# Python Docker Environment

> Please have **Docker** installed prior to executing these steps. `brew install docker`

## Getting Started

- Clone this repository
- Copy it somewhere
- delete the `.git` history folder
- `git init` your project
- Then build your app:

```bash
docker build -t your_app_name_here .
```

Next, run your app!

```bash
docker run -p 4000:80 your_app_name_here
```

This base application is a Flask example that runs on port 80. This docker container is exposing that port 80 via port 4000 locally. Browse to http://0.0.0.0:4000/

## Rebuilding

Each time you update your app, re-build your app:

```bash
docker build -t your_app_name_here .
```

Then re-run:

```bash
docker run -p 4000:80 your_app_name_here
```
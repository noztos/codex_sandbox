# codex_sandbox

This repository is my(noztos) OpenAI codex sandbox, including codex docker container environment.


### clone and build docker images

1. `$ git clone --recurse-submodules git@github.com:noztos/codex_sandbox.git`
1. `$ cd docker`
1. `$ docker compose build`
1. edit OPENAI_API_KEY's value in `docker/docker-compose.yml`

### execution

1. `$ docker compose run --rm codex`

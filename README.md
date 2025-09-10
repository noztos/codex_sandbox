# codex_sandbox

This repository is my(noztos) OpenAI codex sandbox, including codex docker container environment.


### clone and build docker images

1. `$ git clone --recurse-submodules git@github.com:noztos/codex_sandbox.git`
1. `$ cd docker`
1. `$ docker compose build devcontainer`
1. `$ docker compose build codex`

### codex cli execution

1. `$ docker compose run --rm codex`
1. (in container) \
--- sign in to OpenAI ---
1. `$ ssh -R 1455:localhost:1455 -fN host_user_name@host_addr`
1. `$ codex`
1. (in codex prompt) \
--- authentication ---
1. select 'Sign in with ChatGPT', then enter
1. copy `link to authenticate`, then access the URL from **docker host's browser**
1. (operate in **docker host's browser**) sign in to Codex \
you can see `Signed in to Codex` **in browser** and `Welcome to Codex, OpenAI's command-line coding agent` **in codex cli prompt** at signed in completed.

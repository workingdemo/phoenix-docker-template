# Phoenix Docker Template

No need to install elixir, phoenix, or anything locally

Steps:
1. Download this archive and `cd` into the directory
2. `docker compose bash run app` to get a bash prompt inside the docker container
3. `mix phx.new . --app APP_NAME` which will create a new app in the current directory
4. `echo "/_pgdata" >> .gitignore`

Most of this was lifted from: https://elixirforum.com/t/elixir-phoenix-running-a-dev-setup-inside-docker/43269

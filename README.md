# Phoenix Docker Template

No need to install elixir, phoenix, or anything other than docker locally

Steps:
1. Download [this tarred archive](https://github.com/workingdemo/phoenix-docker-template/archive/refs/heads/main.tar.gz)
    * `curl -LJO https://github.com/workingdemo/phoenix-docker-template/archive/refs/heads/main.tar.gz`
    * `tar -zxf phoenix-docker-template-main.tar.gz`
    * `mv phoenix-docker-template-main APP_NAME`
2. `cd` into the directory and run`docker compose bash run app` to get a bash prompt inside the docker container
3. `mix phx.new . -app APP_NAME` which will create a new app in the current directory
4. `echo "/_pgdata" >> .gitignore`
5. edit `config/dev.exs`
    * change the repo hostname from `localhost` to `db`
    * change the endpoint ip from `127.0.0.1` to `0.0.0.0`


Most of this was lifted from: https://elixirforum.com/t/elixir-phoenix-running-a-dev-setup-inside-docker/43269

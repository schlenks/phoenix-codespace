# Phoenix Codespace Template

A Github Codespace template for setting up an [Elixir](https://github.com/elixir-lang/elixir) & [Phoenix Framework](https://github.com/phoenixframework/phoenix) project.

## New Repository Setup

Click the green `Use this template` button to create a repository for your project with the `.devcontainer` folder included. Next, clone it locally to work from your machine or click the green `Code` button to create a new codespace to do cloud editing.

## New Phoenix Project Via Codespace

Codespaces have terminal access allowing you to run commands such as `iex`, `mix`, `node`, and `npm`. 

Run the following command from the terminal:

```
mix phx.new . --app your_app_name
```

**Important notes**: 
1. The `.` in the command instructs `phx.new` to generate the project in the current working directory which will be the _root_ of the repository. 
2. As of Phoenix 1.6, LiveView is enabled by default therefore you no longer  need to pass in the `--live` flag. See [mix phx.new options](https://hexdocs.pm/phoenix/Mix.Tasks.Phx.New.html#module-options) for additional flags to customize your project creation.

## Phonex Project & Codespace Configuration

There are 3 files within the `.devcontainer` folder:
`docker-compose.yml` describes the projects services and dictatest the Elixir, Phoenix & Postgres versions:
- `EX_VERSION` - Elixir Version. Default is _**latest**_
- `PHX_VERSION` - Phoenix Version. Default is _**1.6.2**_
- `db` service - Postgres Version. Default is _**latest**_ via `postgres:latest`

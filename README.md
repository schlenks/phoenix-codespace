# Phoenix Codespace Template

## Setup

Select `Use this template` to create the repository for your project. Now you can either clone it locally are get started coding right away in Codespaces.

Now that your inside your `Dev Container` you have access to `iex`, `mix`, `npm`, and `node`. From here you can generate your Phoenix project doing the following command:
```
mix phx.new . --app your_app_name
```
**Note the "."** Running this command in the current working directory is necessary so it generates in the root of your repository instead of having an additional nested directory.

## Configuration

If you need a specific version of Elixir or Phoenix, open `docker-compose.yml` and change the `VARIANT` or `PHX_VERSION`.

Happy coding!

# ElixirGist

To start your Phoenix server:

  * Run `mix setup` to install and setup dependencies
  * Start Phoenix endpoint with `mix phx.server` or inside IEx with `iex -S mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## Learn more

  * Official website: https://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Forum: https://elixirforum.com/c/phoenix-forum
  * Source: https://github.com/phoenixframework/phoenix

## User mailbox 
  
  * http://localhost:4000/dev/mailbox/

## Commands

  * mix local.hex  ->  Update latest
  * mix archive.install hex phx_new  -> updates to latest phoenix
  * mix phx.new elixir_gist --no-install --binary-id  -> generate project
  * mix phx.gen.auth Accounts User users -> Authentication
  * mix ecto.setup -> database creation
  * mix phx.gen.context Gists Gist gists user_id:references:users name:string description:text markup_text:text
  * mix phx.gen.context Gists SavedGist saved_gists user_id:references:users  gist_id:references:gists
  * mix phx.gen.context Comments Comment comments user_id:references:users  gist_id:references:gists markup_text:text
  * mix ecto.migrate
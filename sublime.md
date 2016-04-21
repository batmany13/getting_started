### Sublime Packages

Here are some useful sublime packages

* [Package Control](https://packagecontrol.io/) - This is the package manager for sublime, this is a must have
* [GitGutter](https://packagecontrol.io/packages/GitGutter) - Show git diffs
* [Emmet](http://docs.emmet.io/) - HTML helper functions
* [Elixir](https://packagecontrol.io/packages/Elixir) - Elixir syntax highlighter
* [ElixirSublime](https://github.com/vishnevskiy/ElixirSublime) - Elixir Auto Completion

### Troubleshooting

__Autocompletion not working__

I had a problem, and it seems like you have to actually modify the config.exs file in ElixirSublime to get it to work, more information [here](https://github.com/vishnevskiy/ElixirSublime/issues/22)

But basically you put this in the config/config.exs

`config :iex,    
    autocomplete_server: IEx.Server`
# evcc completion zsh

Generate the autocompletion script for zsh

## Synopsis

Generate the autocompletion script for the zsh shell.

If shell completion is not already enabled in your environment you will need
to enable it.  You can execute the following once:

```
echo "autoload -U compinit; compinit" >> ~/.zshrc
```

To load completions in your current shell session:

```
source <(evcc completion zsh)
```

To load completions for every new session, execute once:

### Linux:

```
evcc completion zsh > "${fpath[1]}/_evcc"
```

### macOS:

```
evcc completion zsh > $(brew --prefix)/share/zsh/site-functions/_evcc
```

You will need to start a new shell for this setup to take effect.


```
evcc completion zsh [flags]
```

## Options

```
      --no-descriptions   disable completion descriptions
```

## Options inherited from parent commands

```
  -c, --config string   Config file (default "~/evcc.yaml" or "/etc/evcc.yaml")
  -h, --help            Help
      --ignore-db       Run command ignoring service database
  -l, --log string      Log level (fatal, error, warn, info, debug, trace) (default "info")
      --log-headers     Log headers
```

## See also

* [evcc completion](evcc_completion.md)	 - Generate the autocompletion script for the specified shell


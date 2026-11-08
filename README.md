# Homebrew tap for Flightdeck

[Flightdeck](https://github.com/flightdeckhq/flightdeck) is fleet
observability and control for AI coding agents, shipped as one binary.

```sh
brew install flightdeckhq/tap/flightdeck
flightdeck
```

Open the URL it prints. To keep it running in the background:

```sh
brew services start flightdeck
```

The service listens on `127.0.0.1:4000`, keeps its data in
`~/.flightdeck` and logs to `$(brew --prefix)/var/log/flightdeck.log`,
where the start-up block with the dashboard token is.

The formula in `Formula/flightdeck.rb` is written by the release
workflow of the main repository on every stable release; do not edit it
by hand. Issues and pull requests belong in
[flightdeckhq/flightdeck](https://github.com/flightdeckhq/flightdeck).

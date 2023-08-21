# Countdown

<p align="center">
  <br>
  <img src="demo.gif" width="600" alt="Countdown Demo">
  <br>
</p>

<a href="https://webpod.dev/?from=countdown"><img src="https://webpod.dev/img/banner.png" alt="Webpod - deploy JavaScript apps" width="190" align="right"></a>

## Install

```sh
git install https://github.com/tamascsaba/countdown
```

## Build
```sh
go build
```

## Usage

Specify duration in Go format `1h2m3s` or a target time: `02:15pm`, `14:15`.

```sh
countdown 25s
countdown 11:32
```

Add a command with `&&` to run after the countdown.

```sh
countdown 1m30s && say "Hello, world"
```

Count from up from the zero.

```sh
countdown -up 30s
```

Announce (via macOS `say` command) last 10 seconds.

```sh
countdown -say 10s
```

You can change the command like.
```sh
countdown 2m; gtimeout 2s confetty; countdown --up 5m
```

## Key binding

- `Space`: Pause/Resume the countdown.
- `Esc` or `Ctrl+C`: Stop the countdown without running the next command.

## License

[MIT](LICENSE)

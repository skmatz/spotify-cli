# Spotify CLI

`spotify-cli` is a DBus-based Spotify CLI **for Linux**.

This application extracts track information and operates Spotify via DBus (without Spotify API).

## Installation

Get the binary from [GitHub Releases](https://github.com/skmatz/spotify-cli/releases).

Or, if you have Go, you can install `spotify-cli` with the following command.

```console
go get github.com/skmatz/spotify-cli/...
```

## Usage

### Operate

```console
spotify-cli operate --action [action]
```

Available actions are following.

- next
- pause
- play
- play-pause
- previous

### Status

```console
spotify-cli status --format [format]
spotify-cli status --kind [kind]
```

Available formats are following.

- {{ .Album }}
- {{ .AlbumArtist }}
- {{ .Artist }}
- {{ .Playback }}
- {{ .Title }}
- {{ .URL }}

Available kinds are following.

- album
- album-artist
- artist
- playback
- title
- url

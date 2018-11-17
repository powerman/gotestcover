# Go test cover with multiple packages support

## Deprecated

Looks like `go test` now supports this functionality, so there is no
reason to use this tool anymore.

[Original version](https://github.com/pierrre/gotestcover) by Pierre Durand
was [deprecated](https://github.com/pierrre/gotestcover#deprecated).

Differences from original version:
- added support for `-coverpkg`

## Features

- Coverage profile with multiple packages (`go test` doesn't support that)

## Install

`go get github.com/powerman/gotestcover`

## Usage

```sh
gotestcover -coverprofile=cover.out mypackage
go tool cover -html=cover.out -o=cover.html
```

Run on multiple package with:
- `package1 package2`
- `package/...`

Some `go test / build` flags are available.

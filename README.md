# makemake

Automatic `make watch`, in 20 lines of POSIX shell.

## Dependencies

- A POSIX shell and utilities
- GNU make (or a make that behaves in the same way when passed `-p`)
- fswatch

## Installation

makemake is a single shell script, so just drop it somewhere in your
`$PATH` and make it executable:

```console
$ curl -sSLO https://raw.githubusercontent.com/sersorrel/makemake/master/makemake
$ mv makemake ~/.local/bin/
$ chmod +x ~/.local/bin/makemake
```

## Usage

Run makemake from the directory containing your makefile, passing the
name of a target as the argument:

```console
$ makemake all
```

makemake will automatically watch all files that the target depends on,
and rerun make every time one of them changes.

## Bugs

Surely many.

## Contributing

Patches welcome!

## Copyright

Copyright © 2019 Ash Holland. Licensed under the EUPL (1.2 or later).
